# Sensores-Inerciales

## Cross-calibrate
https://medium.com/@lich284/extrinsic-calibration-of-camera-imu-thermal-camera-and-lidar-sensors-code-bf06b208da5b


## Noise Density acel
-----------------------------------------------------------------------------
https://www.allaboutcircuits.com/technical-articles/accelerometer-specifications-measurement-range-sensitivity-and-noise-performance/
https://endevco.com/contentStore/mktgContent/endevco/dlm_uploads/2019/02/Endevco_TP324_REVISED.pdf
https://wilcoxon.com/wp-content/uploads/2020/05/Understanding-the-accelerometer-noise-specification_TN33.pdf
https://www.ctr.unican.es/asignaturas/instrumentacion_5_it/iec_4.pdf
https://biblus.us.es/bibing/proyectos/abreproy/4921/fichero/3.pdf

## Calibration - acc&giros
-----------------------------------------------------------------------------
https://la.mathworks.com/matlabcentral/answers/1774080-creation-of-imu-geometric-model-in-matlab-in-order-to-generate-synthetic-data-accelerometer-and-gyro
https://la.mathworks.com/help/fusion/ug/creating-a-tracking-scenario.html
https://la.mathworks.com/videos/sensor-fusion-part-2-fusing-a-mag-accel-and-gyro-to-estimate-orientation-1569411056638.html

https://github.com/labliscvut/imu_calibration/tree/master
https://github.com/topics/accelerometer-calibration
https://github.com/alrevuelta/sensor-calibration (2 tripletes para el acel)


https://github.com/Razor-AHRS/razor-9dof-ahrs/tree/master/Matlab

(esto NO es mio... buscar referencia)
# MAIN
# Material de Referencia Sensores Inerciales

### IMU-sensor-fusion
Estimación de la orientación via el filtro complementario
https://github.com/abidKiller/IMU-sensor-fusion/tree/main

### https://x-io.co.uk/open-source-imu-and-ahrs-algorithms/

acc and Gyro
https://albertopretto.altervista.org/index.php?mod=02_Publications

-----------

# IMU_sensor_fusion
This repository contains different algorithms for attitude estimation (roll, pitch and yaw angles) from IMU sensors data: accelerometer, magnetometer and gyrometer measurements

File 'IMU_sensors_data.mat' contains real-life sensors measurements, which can be plotted by running the file 'data_plot.m'

File 'accel_mag_inversion.m' solves an opptimization (inverse) problem to find atttitude angles that minimize the error between expected and measured acceleration and magnetic field

File 'dead_reckoning.m' integrates angular rates from gyrometer measurements, with a given initial condition, to obtain attitude angles

File 'complementary_filter.m' uses Matlab function 'complementaryFilter()' to estimate attitude angles from IMU measurements

File 'hamel_mahony.m' implements the nonlinear complementary filter proposed by 'Hamel, Tarek, and Robert Mahony. "Attitude estimation on SO(3) based on direct inertial measurements." Proceedings 2006 IEEE International Conference on Robotics and Automation, 2006. ICRA 2006.. IEEE, 2006.'.

File 'martin_salaun.m' implements the invariant observer proposed in 'Martin, Philippe, and Erwan Salaun. "Invariant observers for attitude and heading estimation from low-cost inertial and magnetic sensors." 2007 46th IEEE Conference on Decision and Control. IEEE, 2007'.

