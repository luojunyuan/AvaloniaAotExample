.nuget\packages\avalonia.win32\11.0.0-rc1.1\lib\net6.0\Avalonia.Win32.dll : warning IL2104: Assembly 'Avalonia.Win32' produced trim warnings. For more information see https://aka.ms/dotnet-illink/libraries

.nuget\packages\avalonia.win32\11.0.0-rc1.1\lib\net6.0\Avalonia.Win32.dll : warning IL3053: Assembly 'Avalonia.Win32' produced AOT analysis warnings.

ILC : Trim analysis warning IL2026: Avalonia.Data.Core.Plugins.ObservableStreamPlugin.ObservableStreamPlugin(): Using member 'Avalonia.Data.Core.Plugins.ObservableStreamPlugin.GetBoxObservable(Type)' which has 'RequiresUnreferencedCodeAttribute' can break functionality when trimming application code. StreamPlugin might require unreferenced code.

ILC : Trim analysis warning IL2026: Avalonia.Data.Core.Plugins.ObservableStreamPlugin.ObservableStreamPlugin(): Using member 'Avalonia.Data.Core.Plugins.ObservableStreamPlugin.GetBoxObservable()' which has 'RequiresUnreferencedCodeAttribute' can break functionality when trimming application code. StreamPlugin might require unreferenced code.

.nuget\packages\avalonia\11.0.0-rc1.1\lib\net6.0\Avalonia.Base.dll : warning IL3053: Assembly 'Avalonia.Base' produced AOT analysis warnings. 

.nuget\packages\runtime.win-x64.microsoft.dotnet.ilcompiler\8.0.0-preview.4.23259.5\framework\System.Linq.Expressions.dll : warning IL3053: Assembly 'System.Linq.Expressions' produced AOT analysis warnings.

---

目前 Avalonia 11.1.0 AOT net8 存在的警告


```powershell
# trim warnings
C:\Users\CYCY\.nuget\packages\reactiveui\18.3.1\lib\net6.0\ReactiveUI.dll : warning IL2104: Assembly 'ReactiveUI' produced trim warnings. For more information see https://aka.ms/dotnet-illink/libraries

C:\Users\CYCY\.nuget\packages\system.reactive\5.0.0\lib\net5.0\System.Reactive.dll : warning IL2104: Assembly 'System.Reactive' produced trim warnings. For more information see https://aka.ms/dotnet-illink/libraries

C:\Users\CYCY\.nuget\packages\avalonia.win32\11.1.0\lib\net8.0\Avalonia.Win32.dll : warning IL2104: Assembly 'Avalonia.Win32' produced trim warnings. For more information see https://aka.ms/dotnet-illink/libraries

C:\Users\CYCY\.nuget\packages\avalonia\11.1.0\lib\net8.0\Avalonia.Base.dll : warning IL2104: Assembly 'Avalonia.Base' produced trim warnings. For more information see https://aka.ms/dotnet-illink/libraries

# AOT analysis warnings
C:\Users\CYCY\.nuget\packages\avalonia\11.1.0\lib\net8.0\Avalonia.Base.dll : warning IL3053: Assembly 'Avalonia.Base' produced AOT analysis warnings.

C:\Users\CYCY\.nuget\packages\runtime.win-x64.microsoft.dotnet.ilcompiler\8.0.7\framework\System.Linq.Expressions.dll :
 warning IL3053: Assembly 'System.Linq.Expressions' produced AOT analysis warnings.

# 需注意默认转换器
ILC : Trim analysis warning IL2026: Avalonia.Data.Core.TargetTypeConverter.DefaultConverter.TryConvert(Object,Type,Cult
ureInfo,Object&): Using member 'System.ComponentModel.TypeDescriptor.GetConverter(Type)' which has 'RequiresUnreferencedCodeAttribute' can break functionality when trimming application code. Generic TypeConverters may require the generic types to be annotated. For example, NullableConverter requires the underlying type to be DynamicallyAccessedMembers All.

```
