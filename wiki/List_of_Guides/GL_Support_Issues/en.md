The next large release of osu! (coming in August-September 2015) removes DirectX support in order to simplify our framework. If you are seeing this page, it means you are likely unable to play osu! on your current system when the new release goes live. This page has common solutions for problems that we have found. Please read through and try them out!

Missing or old Drivers
======================

If you don't have correct graphics drivers installed, Windows will use a "Basic Display Adapter" fallback driver, which **works** for DirectX games but is very slow. It doesn't work at all for OpenGL, so we will need to make sure you have correct drivers.

First, let's check if this applies to you:

-   Right click on My Computer and choose Properties from the dropdown, or press WinKey+Break on your keyboard.
-   Choose Device Manager on the left.

Check whether you are using Microsoft Basic Display Adapter as per the following diagram:

<img src="Devicemanager.png" title="Devicemanager.png" alt="Devicemanager.png" width="800" />

Please find drivers for your card from your manufacturer's website. Here are some common links:

-   AMD / ATI: <http://support.amd.com/en-us/download>
-   NVIDIA: <http://www.nvidia.com/Download/index.aspx?lang=en-us>
-   Intel: <https://downloadcenter.intel.com/search?keyword=2nd+Generation+Intel%C2%AE+Core%E2%84%A2+Processors+with+Intel%C2%AE+HD+Graphics+3000%2F2000>

Wrong bit depth
===============

Your drivers could be installed properly but your colour bit depth may be wrong. Windows will fallback to generic drivers [when colour bit depth is not 32bpp](https://www.opengl.org/discussion_boards/showthread.php/145008-Why-my-OpenGL-program-uses-Microsoft-GDI-renderer-instead-of-my-GeForce-5200). Changing [colour bit depth to 32bpp will fix this.](http://windows.microsoft.com/en-us/windows/getting-best-display-monitor#getting-best-display-monitor&section_2)

Additional Help
===============

If your problem isn't fixed by the solutions above, then please open a thread in the [help forum](https://osu.ppy.sh/forum/5) with the output of [this program](http://www.realtech-vr.com/glview/download.php) and your gl\_info.txt if you are on the Cutting Edge stream.
