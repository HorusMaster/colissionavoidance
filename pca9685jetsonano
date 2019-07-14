from pca9685_driver import Device

def set_duty_cycle(pwmdev, channel, dt):
    """    
    @channel Channel or PIN number in PCA9685 to configure 0-15
    @dt desired duty cycle
    """
    val = (dt*4095)//100
    pwmdev.set_pwm(channel,val)

pca9685 = Device(0x40, 1)

# Set duty cycle
#pca9685.set_pwm(0, 2047)

# set pwm freq
pca9685.set_pwm_frequency(60)

set_duty_cycle(pca9685,0,7)
