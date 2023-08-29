<b>Connect lock app android or ios, not gateway!</b>
<p>Remove lock geteway!</p>
<p>Or delete device app and gateway</p>
<p>Disconect power gateway!</p>
<p>And new connect in app</p>
<p>Turn off bluetooth in device</p>
<p>Add in home assistant.</p>
<p>Reconect battery</p>

<br>

<b>Add smart lock Moes R2</b>

<p>add configuration.yaml</p>
<div class=WordSection1>

<p class=MsoNormal><span class=GramE><span lang=EN-US style='mso-ansi-language:
EN-US'>lock</span></span><span lang=EN-US style='mso-ansi-language:EN-US'>:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>  </span>- <span class=GramE>platform</span>: template<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>    </span><span class=GramE>name</span>: Garage door<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>    </span>value_template: &quot;{<span class=GramE>{
is</span>_state('binary_sensor.bf75d830c48449b139xmbm_lock_motor_state', 'off')
}}&quot;<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>    </span><span class=GramE>lock</span>:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- <span class=GramE>service</span>:
switch.turn_off<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span><span class=GramE>data</span>: {}<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span><span class=GramE>target</span>:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>entity_id:
switch.bf75d830c48449b139xmbm_manual_lock<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- delay:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>hours: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>minutes: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>seconds: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>milliseconds: 300<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- service: switch.turn_on<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>         </span><span
style='mso-spacerun:yes'>   </span>data: {}<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span>target:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>entity_id:
switch.bf75d830c48449b139xmbm_manual_lock<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>    </span>unlock:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- service: switch.turn_off<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span>data: {}<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span>target:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>entity_id:
switch.bf75d830c48449b139xmbm_manual_unlock<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- delay:<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>hours: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>minutes: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>seconds: 0<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span>milliseconds: 300<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>          </span>- service: switch.turn_on<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span>data: {}<o:p></o:p></span></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>            </span></span><span class=SpellE>target</span>:<o:p></o:p></p>

<p class=MsoNormal><span lang=EN-US style='mso-ansi-language:EN-US'><span
style='mso-spacerun:yes'>              </span><span class=SpellE>entity_id</span>:
switch.bf75d830c48449b139xmbm_manual_unlock<o:p></o:p></span></p>

</div>


# Home Assistant support for Tuya BLE devices

## Overview

This integration supports Tuya devices connected via BLE.

_Inspired by code of [@redphx](https://github.com/redphx/poc-tuya-ble-fingerbot)_

## Installation

Place the `custom_components` folder in your configuration directory (or add its contents to an existing `custom_components` folder). Alternatively install via [HACS](https://hacs.xyz/).

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=PlusPlus-ua&repository=ha_tuya_ble&category=integration)

## Usage

After adding to Home Assistant integration should discover all supported Bluetooth devices, or you can add discoverable devices manually.

The integration works locally, but connection to Tuya BLE device requires device ID and encryption key from Tuya IOT cloud. It could be obtained using the same credentials as in official Tuya integration. To obtain the credentials, please refer to official Tuya integration [documentation](https://www.home-assistant.io/integrations/tuya/)

## Supported devices list

* Fingerbots (category_id 'szjqr')
  + Fingerbot (product_ids 'ltak7e1p', 'y6kttvd6', 'yrnk7mnn', 'nvr2rocq', 'bnt7wajf', 'rvdceqjh', '5xhbk964'), original device, first in category, powered by CR2 battery.
  + Adaprox Fingerbot (product_id 'y6kttvd6'), built-in battery with USB type C charging.
  + Fingerbot Plus (product_ids 'blliqpsj', 'ndvkgsrm', 'yiihr7zh', 'neq16kgd'), almost same as original, has sensor button for manual control.
  + CubeTouch 1s (product_id '3yqdo5yt'), built-in battery with USB type C charging.
  + CubeTouch II (product_id 'xhf790if'), built-in battery with USB type C charging.

  All features available in Home Assistant, programming (series of actions) is implemented for Fingerbot Plus.
  For programming exposed entities 'Program' (switch), 'Repeat forever', 'Repeats count', 'Idle position' and 'Program' (text). Format of program text is: 'position\[/time\];...' where position is in percents, optional time is in seconds (zero if missing).

* Temperature and humidity sensors (category_id 'wsdcg')
  + Soil moisture sensor (product_id 'ojzlzzsw').

* CO2 sensors (category_id 'co2bj')
  + CO2 Detector (product_id '59s19z5m').

* Smart Locks (category_id 'ms')
  + Smart Lock (product_id 'ludzroix', 'isk2p555').

* Climate (category_id 'wk')
  + Thermostatic Radiator Valve (product_ids 'drlajpqc', 'nhj2j7su').

* Smart water bottle (category_id 'znhsb')
  + Smart water bottle (product_id 'cdlandip')

* Irrigation computer (category_id 'ggq')
  + Irrigation computer (product_id '6pahkcau')

## Support project

I am working on this integration in Ukraine. Our country was subjected to brutal aggression by Russia. The war still continues. The capital of Ukraine - Kyiv, where I live, and many other cities and villages are constantly under threat of rocket attacks. Our air defense forces are doing wonders, but they also need support. So if you want to help the development of this integration, donate some money and I will spend it to support our air defense.
<br><br>
<p align="center">
  <a href="https://www.buymeacoffee.com/3PaK6lXr4l"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy me an air defense"></a>
</p>

