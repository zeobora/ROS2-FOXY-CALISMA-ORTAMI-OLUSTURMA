# ROS2-FOXY-WORKSPACE

ÇALIŞMA ORTAMININ OLUŞTURULMASI


1- “mkdir -p ~/ros2_ws/src” komutu ile klasörler oluşturuldu.

2- “cd ~/ros2_ws/src” komutu ile belirtilen dizine gidildi.

3- “git clone https://github.com/ros/ros_tutorials.git -b foxy-devel” komutu ile belirtilen dizine GITHUB’dan depo indirildi.

4- “cd..” komutu ile bir üst dizine gidildi.

5- “rosdep install -i --from-path src --rosdistro foxy -y” komutu ile paket bağımlılıklarını çözüyoruz. Bu komutu çalıştırdıktan sonra terminalde “All required rosdeps installed successfully” yazıyor olmalıdır.

6- “sudo apt install python3-colcon-common-extensions” komutu ile calcon’u kurunuz.

7- “pip install pytest-rerunfailures” komutu ile gerekli bir paketi kurunuz.

8- “colcon build” komutu ile çalışma ortamının oluşturunuz. Bu komutu çalıştırdıktan sonra aşağıdaki gibi bir şey yazıyor olmalıdır:

Starting >>> turtlesim
Finished <<< turtlesim [5.49s]
Summary: 1 package finished [5.58s]

9- ros2_ws dizinine gidip “ls” komutunu çalıştırdığımızda aşağıdakileri görüyorsak çalışma ortamını oluşturduk demektir:

build  install  log  src

10- .bashrc dosyasını “nano ~/.bashrc” komutu ile açıp “source /home/zeobora/ros2_ws/install/setup.bash” satırını eklemelisiniz.

11- Artık terminali kapatıp açtığımızda ve “ros2 run turtlesim turtlesim_node” komutunu çalıştırığımızda çalışıyor olmalıdır.
