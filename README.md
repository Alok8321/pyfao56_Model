## pyfao56 Model
pyfao56 is a model for estimating crop water use and irrigation scheduling based on FAO-56 dual crop coefficient approach. The pyfao56 model is implemented in Python and provides a convenient way to calculate evapotranspiration. It takes input parameters such as meteorological data (e.g., temperature, humidity, wind speed) and crop coefficients to compute ET rates for specific crop types and land surfaces.
In this model I used autoirrigate class to get Evaporation, Transpiration, Crop Evapotranspiration, Irrigation, Deep percolation etc.
## Autoirrigate Class
While users have the flexibility to define irrigation management schedules manually using the Irrigation class, the AutoIrrigate class within pyfao56 offers an automated approach for computing irrigation schedules. The AutoIrrigate class provides so many parameters that can be used to customize automatic irrigation scheduling in pyfao56. Parameters for controlling autoirrigation timing include the start and end dates for the autoirrigation time period, day(s) of the week that irrigation is permitted, consideration of forecasted precipitation events, managment allowed depletion, the transpiration reduction coefficient (Ks) below a critical value, and days since last irrigation or watering event.
## Steps for Modeling
1. Install pyfao56
2. Import pyfao56 package
3. Specify the model parameters
4. Specify the weather information
5. Run the daily soil water balance model with autoirrigation
6. Save the output
## Model Parameters
    Kcbini : float
        Kcb Initial (FAO-56 Table 17)
    Kcbmid : float
        Kcb Mid (FAO-56 Table 17)
    Kcbend : float
        Kcb End (FAO-56 Table 17)
    Lini : int
        Length Stage Initial (days) (FAO-56 Table 11)
    Ldev : int
        Length Stage Development (days) (FAO-56 Table 11)
    Lmid : int
        Length Stage Mid (days) (FAO-56 Table 11)
    Lend : int
        Length Stage End (days) (FAO-56 Table 11)
    hini : float
        Plant Height Initial (m)
    hmax : float
        Plant Height Maximum (m) (FAO-56 Table 12)
    thetaFC : float
        Volumetric Soil Water Content, Field Capacity (cm3/cm3)
    thetaWP : float
        Volumetric Soil Water Content, Wilting Point (cm3/cm3)
    theta0 : float
        Volumetric Soil Water Content, Initial (cm3/cm3)
    Zrini : float
        Rooting Depth Initial (m)
    Zrmax : float
        Rooting Depth Maximum (m) (FAO-56 Table 22)
    pbase : float
        Depletion Fraction (p) (FAO-56 Table 22)
    Ze : float
        Depth of surface evaporation layer (m) (FAO-56 Table 19 & p144)
    REW : float
        Total depth Stage 1 evaporation (mm) (FAO-56 Table 19)
    CN2 : int
        Curve Number for AWC II (ASCE (2016), Table 14-3, p452)
    comment : str, optional
        User-defined file descriptions or metadata (default = '')
    tmstmp : datetime
        Time stamp for the class
## Weather Information
1.kjskdj
,l,dl
smdmsc


