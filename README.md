Hook-library-calls
==================

Mark windows/linux hook.

windows下 HOOK Win32 API 可直接用微软 detours库http://research.microsoft.com/en-us/projects/detours/（网上有很多资料），替换WAPI

linux下 Introduction to Reverse Engineering Software in Linux，利用LD_PRELOAD环境变量给glibc库函数加钩子，
它可以影响程序的运行时的链接（Runtimelinker），它允许你定义在程序运行前优先加载的动态链接库。这个功能主要就是用来有选择性的载入Linux操作系统不同动态链接库中的相同函数。通过这个环境变量，我们可以在主程序和其动态链接库的中间加载别的动态链接库，甚至覆盖正常的函数库。
