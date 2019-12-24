# klte-stuff-G900F-
Samsung Galaxy S5 SM-G900F klte


----------
- name: Samsung Galaxy S5 (Qcom)
  id: klte
  codenames:
    - klte
    - kltecan
    - kltedv
    - kltespr
    - kltetmo
    - klteusc
    - kltevzw
    - kltexx
    - kltekdi
  architecture: armeabi-v7a

  block_devs:
    base_dirs:
      - /dev/block/platform/msm_sdcc.1/by-name
    system:
      - /dev/block/platform/msm_sdcc.1/by-name/system
      - /dev/block/mmcblk0p23
    cache:
      - /dev/block/platform/msm_sdcc.1/by-name/cache
      - /dev/block/mmcblk0p24
    data:
      - /dev/block/platform/msm_sdcc.1/by-name/userdata
      - /dev/block/mmcblk0p26
    boot:
      - /dev/block/platform/msm_sdcc.1/by-name/boot
      - /dev/block/mmcblk0p15
    recovery:
      - /dev/block/platform/msm_sdcc.1/by-name/recovery
      - /dev/block/mmcblk0p14

  boot_ui:
    supported: true
    flags:
      - TW_QCOM_RTC_FIX
      - TW_HAS_DOWNLOAD_MODE
    pixel_format: RGBX_8888
    graphics_backends:
      - fbdev
    theme: portrait_hdpi
    brightness_path: /sys/devices/mdp.0/qcom,mdss_fb_primary.191/leds/lcd-backlight/brightness
    max_brightness: 255
    default_brightness: 162
