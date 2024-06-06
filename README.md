# MSBuildApp
msbuild 扩展

# TargetFrameworks 
针对 TargetFramework 进行扩展，在ui开发上，能支持其他框架库进行多框架支持，如针对skia上进行ui开发，对wasm上进行ui开发，因要引用不同的包来实现ui，所以dll是不同的

原理有两种，一种是扩展TargetFramework，一种是吧生成的包丢到nuget包目录的其他文件夹，在生成输出dll时替换net8.0框架库的dll，到对应的ui扩展库net8.0/skia 这样的dll上

