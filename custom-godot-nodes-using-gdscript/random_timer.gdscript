@tool
extends Timer
class_name RandomTimer

"""
An implementation of the timer node, which uses a random time, rather than a
set time.
"""

@export var min_time = 0.0
@export var max_time = 1.0

func _validate_property(property):
	if property.name == "wait_time":
		property.usage &= ~PROPERTY_USAGE_EDITOR
		
func _get_random_time():
	return randf_range(min_time, max_time)
	
func _on_timeout():
	self.wait_time = _get_random_time()
	
func _ready() -> void:
	self.timeout.connect(_on_timeout)
	self.wait_time = _get_random_time()
