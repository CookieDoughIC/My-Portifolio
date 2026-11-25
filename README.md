# My-Portifolio

Currently studying programming in TEC
im interested in learning in general.
I recently started learning how to make games in godot.
- Currently working on Tower Defenses.
- I wanna learn more about different languages.
- Improve my knowledge in C#.
extends Node


func _ready():
	get_node("MainMenu/M/VB/NewGame").connect("pressed",Callable(self,"on_new_game_pressed"))
	get_node("MainMenu/M/VB/Quit").connect("pressed",Callable(self,"on_quit_pressed"))


func on_new_game_pressed():
	get_tree().change_scene_to_file("res://Scenes/MainScenes/game_scene.tscn")
	
func on_quit_pressed():
	get_tree().quit()

- [ ] TowerDefense Færdigt
