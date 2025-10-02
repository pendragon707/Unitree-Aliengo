# Unitree-Aliengo

Модель AlienGo - это промышленный четырехопорный робот-собака, являющаяся программно-аппаратным комплексом для профессиональной разработки и создания пользовательского функционала. 

Робот поставляется вместе с SDK, так же имеется программный слой для управления из под фреймворка ROS (ROS Noetic).

## Код для работы с Aliengo

1. Официальное сдк
https://github.com/unitreerobotics/unitree_legged_sdk/tree/Aliengo	

2. Проект для запуска скриптов и рл-политик на робособаке через сдк + в симуляторе mujoco (официальное сдк есть в проекте rl_go1 в качестве подмодуля):
https://github.com/pendragon707/rl_go1

3. RMA
Проект для обучения RL-политик для Unitree Aliengo
https://github.com/pendragon707/raisimLib


## Полезные материалы
Документация и разное
https://drive.google.com/drive/folders/1LXvSTHD2Fv9Eu8THsu8kQpHDs2XjbYZg?usp=sharing
	
### Про сдк

- Официальное сдк для управления Unitree Aliengo (оно есть в проекте rl_go1 в качестве подмодуля):
https://github.com/unitreerobotics/unitree_legged_sdk/tree/Aliengo	

- Инструкция на русском (в том числе про управление с пульта)
https://robodocs.3logic.ru/docs/Unitree%20Robotics/AlienGo/aliengo_general.html

- Документация
https://unitree-docs.readthedocs.io/en/latest/Aliengo/AlienGo.html

- Документация про сдк моторов
https://support.unitree.com/home/en/Motor_SDK_Dev_Guide/control_mode
	 			 			
### Про РЛ
- Воркшоп по обучению и запуску рл-политики на робособаке
Используется симулятор IsaacGym, робособаку учат сидеть
https://github.com/StarkitRobots/workshop_legged_gym/tree/workshop

https://drive.google.com/file/d/1P74rLRLfFPB3tsmI4Sh1NhqNrNqzQpDX/view?usp=sharing

- Примеры с go1 в mujoco.
Можно изучить, какие награды используются, чтобы научить робособаку ходить на двух лапах и ходить по джойстику
https://colab.research.google.com/github/google-deepmind/mujoco_playground/blob/main/learning/notebooks/locomotion.ipynb
https://github.com/google-deepmind/mujoco_playground/tree/main/mujoco_playground/_src/locomotion/go1

- URDF 
Отсюда можно брать модели роботов, чтобы после на основе них обучать RL-политики

Gazebo
https://github.com/unitreerobotics/unitree_ros/tree/master/robots

https://github.com/unitreerobotics/unitree_rl_gym/tree/main/resources/robots

Mujoco
https://github.com/unitreerobotics/unitree_mujoco/tree/main/unitree_robots