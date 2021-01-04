동작 전압의 상한 값과 하한 값입니다.  
장치에 현재 인가된 전압을 나타내는 [Present Input Voltage(144)](#present-input-voltage144)가 Max Voltage Limit(32)와 Min Voltage Limit(34)의 범위를 벗어날 경우,  
[Hardware Error Status(70)](#hardware-error-status70)의 Voltage Range Error Bit(0x01)와 Hardware Error Bit(0x80)이 설정됩니다.  
[Shutdown(63)]에 Input Voltage Error Bit(0x10)가 설정된 경우, [Torque Enable(64)](#torque-enable64)은 ‘0’이 되고 Torque가 OFF 됩니다.  
자세한 설명은 [Shutdown(63)]을 참고하세요.

{% if page.product_group=='dxl_xl430' %}

|     단위      |   범위   |   상세 설명    |
|:-------------:|:--------:|:--------------:|
| About 0.1 [V] | 65 ~ 140 | 6.5 ~ 14.0 [V] |

{% elsif page.product_group=='xl330' %}

|     단위      |   값    |     설명      |
|:-------------:|:-------:|:-------------:|
| About 0.1 [V] | 31 ~ 70 | 3.1 ~ 7.0 [V] |

{% else %}

|     단위      |   범위   |   상세 설명    |
|:-------------:|:--------:|:--------------:|
| About 0.1 [V] | 95 ~ 160 | 9.5 ~ 16.0 [V] |

{% endif %}
