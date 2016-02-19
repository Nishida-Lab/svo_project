# SVO project

### 概要
SVOアルゴリズムを試す際に、fpsの高いカメラが現実では手に入りにくいとの声がありましたので、  
Gazebo上で要求を満たすものを作ってみました。  

移動物体等は必要に応じて追加してゆく予定です。

### 使い方
#### 前提
ROSがインストールされている必要があります。  
そのあたりについては、本リポジトリでは触れませんので、あしからず。
#### インストール
1. clone
   ```bash
   cd <catkin_ws>/src/
   git clone https://github.com/Nishida-Lab/svo_project.git
   ```
   
2. rosdep
   ```bash
   cd <catkin_ws>
   rosdep install -i --from-paths src
   ```

3. パス通し
   ```bash
   cd <catkin_ws>
   source devel/setup.bash
   ```

#### 起動手順
1. Gazeboの起動
   ```bash
   roslaunch model_gazebo model_empty_world.launch
   ```

2. svoの起動

### 最後に
Gazebo辺りのことがわからなかったら、[RyodoTanaka](http://github.com/RyodoTanaka)まで、よろしくお願いします。
