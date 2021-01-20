# Multiwii-2020-update

just open multiwii.ino using the Arduino IDE 
Adjust the Config.h parameters according to your drone type and sensors
compile and build into your selected arduino board from Tool menu.




Note : some changes updated on this additional sensors implementation and Wish list looking for contributors 



/***************************    independent sensors    ********************************/
      
// WishList for contribution  //  
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
        
//Implemented sensors as of 2020//     
      AK8963
      BMP280
      QMC5883
      
      
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
