# Multiwii-2020-update

just open multiwii.ino using the Arduino IDE 
Adjust the Config.h parameters according to your drone type and sensors
compile and build into your selected arduino board from Tool menu.

2021 update note Note for 

for complete ready to use set for arduino drone and Synerduino shield you can simply download 
synerduinokwad3.zip 

with the current sensors for multiwii as of 2020-2021
------------->
Magnetometer HMC5883 and HMC5843 are discontinued - pls migrate to QMC5883 and MMC5883 
------------->
Barometer BMP085 and 180BMP are hard to come by as this is written - Pls migrate to BMP280
------------->
GYRO and  ACC MPU6050   combo + ACC (Possible support for MPU9250)




Note : some changes updated on this additional sensors implementation and Wish list looking for contributors 



/***************************    independent sensors    ********************************/
      
// WishList for contribution for those who wish to add hit me up here on discussions //  
      QMC6310
      RM3100
      ICM-20948
      QMA6981
      LSM6DS33
      LIS3MDL
      BME280
      MMC3416
      LSM303
      BMM150
      BMP388
      BMP380
        
//Implemented sensors as of 2020//     
      AK8963
      BMP280
      QMC5883
      MMC5883
      
      
      /* I2C gyroscope */
      //#define WMP
      //#define ITG3050
      //#define ITG3200
      //#define MPU3050
      //#define L3G4200D
      //#define MPU6050       //combo + ACC (Possible support for MPU9250)
      //#define LSM330        //combo + ACC
      
      /* I2C accelerometer */
      //#define MMA7455
      //#define ADXL345
      //#define BMA020
      //#define BMA180
      //#define BMA280
      //#define LIS3LV02
      //#define LSM303DLx_ACC
      //#define MMA8451Q

      /* I2C barometer */
      //#define BMP085
      //#define BMP280
      //#define MS561101BA
      

      /* I2C magnetometer */
      //#define HMC5843
      //#define HMC5883
      //#define QMC5883
      //#define AK8975
      //#define AK8963
      //#define MAG3110
      //#define MMC5883
      
      
      # Synerduino Kwad3
      Multiwiibase update for both GY91 and GY801 MMC sensor 10 DOF module
      
     

/***************************    Dec19 2021 Update    ********************************/ 
      
      # Synerduino Kwad3 1.8.16
      noted by JerwinJohn  this fixes the UBLOX GPS Array error when compiling using the Arduino 1.8.16 -1.8.18 -2.0.0 Arduino IDE versions
      uint8_t bytes[]; was change to  uint8_t bytes[128]; 
      
      in GPS.cpp 
      // Receive buffer
      static union {
  ubx_nav_posllh posllh;
  ubx_nav_solution solution;
  ubx_nav_velned velned;
  uint8_t bytes[128];
 } _buffer;
 
 
      
      
