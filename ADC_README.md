# ADC_readme
*STEP 1: First of all Enable the Beagleboard black for ADC input
<ol>
  <li>Go to *sys*, then to *devices*, then to **bone_capemgr.* (* refer to the number. In my case it was 11)**, then to    **slots**. Check out the values if any. </li>
  <li>The initialize the Beaglebone black with the values. DO **echo cape-bone-iio > /sys/devices/bone_capemgr.*/slots</li>
  <li>Check out the **cat /sys/devices/ocp.2/helper.11/AIN1** to check out the values from first ADC. Bear in mind that *ocp.2 could be ocp.3 or any other values. So replace the appropriate value there. Similarly *helper.11* in my case could be *helper.12* or any other value. So check out the value and replace the appropirate values. </li>
</ol>
