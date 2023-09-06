# Quick.AvaloniaFonts.SourceHanSansCN
* SourceHanSansCN fonts for Avalonia
* Full version： [![NuGet Downloads](https://img.shields.io/nuget/dt/Quick.AvaloniaFonts.SourceHanSansCN.svg)](https://www.nuget.org/packages/Quick.AvaloniaFonts.SourceHanSansCN/)
* Slim version： [![NuGet Downloads](https://img.shields.io/nuget/dt/Quick.AvaloniaFonts.SourceHanSansCN.Slim.svg)](https://www.nuget.org/packages/Quick.AvaloniaFonts.SourceHanSansCN.Slim/)

How to use
-------------
Replace ***.WithInterFont()*** to ***.WithFont_SourceHanSansCN()*** in Program.cs

Example
-------------
```
using Avalonia;
using System;

namespace TestApp;

class Program
{
    // Initialization code. Don't use any Avalonia, third-party APIs or any
    // SynchronizationContext-reliant code before AppMain is called: things aren't initialized
    // yet and stuff might break.
    [STAThread]
    public static void Main(string[] args) => BuildAvaloniaApp()
        .StartWithClassicDesktopLifetime(args);

    // Avalonia configuration, don't remove; also used by visual designer.
    public static AppBuilder BuildAvaloniaApp()
        => AppBuilder.Configure<App>()
            .UsePlatformDetect()
            //.WithInterFont()()
            .WithFont_SourceHanSansCN()
            .LogToTrace();
}
```
