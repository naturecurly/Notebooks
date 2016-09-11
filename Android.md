**1.** 避免在Fragment的onCreate()和onDestroy()方法中调用getActivity()方法，因为旋屏时会返回不同的值。

**2.** 使用Camera2的基本步骤：
    1. 先创建TextureView或SurfaceView
    2. 设置相机的参数，如获取相机ID，设置相机尺寸等
    3. 打开相机
    4. 创建requestSession以处理request
