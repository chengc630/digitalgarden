---
{"dg-publish":true,"permalink":"/opengl/open-gl-open-gl-sukhoi27smk-csdn/","tags":["OpenGL版本与OpenGL扩展机制"]}
---


# OpenGL版本与OpenGL扩展机制_sukhoi27smk的博客-CSDN博客

> ## Excerpt
> 1 opengl的版本区别（在opengl官方文档中有详细说明）    针对Opengl不同版本的升级是主要是扩展指令集。    现在版本是4.0啦1.1 opengl1.11995年，SGI推出了更为完善的OpenGL 1.1版本。OpenGL 1.1的性能比1.0版提高甚多。其中包括改进打印机支持，在增强元文件中包含OpenGL的调用，顶点数组的新特性，提高顶点位置、法线、颜色、色彩指...

---
![photos/OpenGL版本与OpenGL扩展机制_sukhoi27smk的博客-CSDN博客/reprint.png](/img/user/photos/OpenGL%E7%89%88%E6%9C%AC%E4%B8%8EOpenGL%E6%89%A9%E5%B1%95%E6%9C%BA%E5%88%B6_sukhoi27smk%E7%9A%84%E5%8D%9A%E5%AE%A2-CSDN%E5%8D%9A%E5%AE%A2/reprint.png)

**1 opengl****的版本区别（在****opengl****官方文档中有详细说明）**  
    针对[Opengl](https://so.csdn.net/so/search?q=Opengl&spm=1001.2101.3001.7020)不同版本的升级是主要是扩展指令集。  
    现在版本是4.0啦  
1.1 opengl1.1  
1995年，SGI推出了更为完善的OpenGL 1.1版本。OpenGL 1.1的性能比1.0版提高甚多。其中包括改进打印机支持，在增强元文件中包含OpenGL的调用，顶点[数组](https://so.csdn.net/so/search?q=%E6%95%B0%E7%BB%84&spm=1001.2101.3001.7020)的新特性，提高顶点位置、法线、颜色、色彩指数、纹理坐标、多边形边缘标识的传输速度，引入了新的纹理特性等等。  
1.2 opengl1.3  
2001年8月，ARB发布OpenGL 1.3规范，它增加了立方纹理贴图、纹理环境、多重采样、纹理框架压缩等扩展指令，但是改进程度非常有限。   
1.3 opengl1.4  
2002年7月，ARB正式发布OpenGL 1.4，它也只加入了深度纹理／阴影纹理、顶点设计框架、自动纹理贴图等简单的功能。   
1.3 opengl1.5  
2003年的7月，ARB公布OpenGL 1.5规范。OpenGL 1.5内包含ARB制定的“正式扩展规格绘制语言”（OpenGL Shading Language v1.0），该语言用于着色对象、顶点着色、片断着色等扩展功能，同时也将作为下一代OpenGL 2.0版本的内核。OpenGL 1.5的变化还增加了顶点缓冲对象（可提高透视性能）、非乘方纹理(可提高纹理内存的使用效率)以及阴影功能、隐蔽查询功能等等。其主要内容包括  
l         顶点Buffer Object：进行顶点配列方式可以提高透视性能  
l         Shadow功能：增加用来比较Shadow映射的函数  
l         隐蔽查询(QUERY)：为提高Curling性能采用非同步隐蔽测试  
l         非乘方纹理(Texture)：提高mipmap等纹理内存的使用效率  
l         OpenGL Shading Language v.1.0：用于着色(shader)对象、顶点着色以及片断着色技术(fragment shader )的扩展功能   
1.4 opengl2.0  
OpenGL 1.0推出后的相当长的一段时间里，OpenGL唯一做的只是增加了一些扩展指令集，这些扩展指令是一些绘图功能，像是ClearCoat、Multisample、视频及绘图的整合工具(某些是通过OpenML的努力而开发出来的，它本身属于OpenGL ARB扩展指令之一。  
已经推出opengl2.0。OpenGL 2.0将在OpenGL 1.3基础上进行修改扩充、但它将有下面五个方面的重大改进：①复杂的核心被彻底精简；②完全的硬件可编程能力；③改进的内存管理机制、支持高级像素处理；④扩展至数字媒体领域，使之跨越高端图形和多媒体范畴；⑤支持嵌入式图形应用。  
为了在获得强大功能的同时保持理想的兼容性，OpenGL 2.0经历以下两个发展阶段：第一个阶段注重兼容能力和平滑过渡，为此，OpenGL 2.0核心将在精简后的OpenGL 1.3功能模块的基础上加上可完全兼容的新功能共同组成，这种做法在满足兼容性的同时，还可将原有OpenGL中数量众多、且相互纠缠不清的扩展指令进行彻底精简。 第一阶段的任务只是为了过渡，而第二阶段才是OpenGL 2.0的真正成熟期。此时，ARB将合成出一个“纯OpenGL 2.0”内核，纯内核将包含更多新增加的“精简型API函数”，这些函数具有完全的可编程特性、结构简单高效、功能强大且应用灵活。除了完成这项任务外，ARB组织还得指导开发商抛弃繁琐的OpenGL 1.X、转用更具弹性的“纯OpenGL 2.0”。   
2 OpenGL扩展（OpenGL Extensions）  
OpenGL和Direct3D比较起来，最大的一个长处就是其扩展机制。硬件厂商开发出一个新功能，可以针对新功能开发OpenGL扩展，软件开发人员通过这个扩展就可以使用新的硬件功能。所以虽然显卡的发展速度比OpenGL版本更新速度快得多，但程序员仍然可以通过OpenGL使用最新的硬件功能。而Direct3D则没有扩展机制，硬件的新功能要等到微软发布新版DirectX后才可能支持。  
    OpenGL扩展也不是没有缺点，正因为各个硬件厂商都可以开发自己的扩展，所以扩展的数目比较大，而且有点混乱，有些扩展实现的相同的功能，可因为是不同厂商开发的，接口却不一样，所以程序中为了实现这个功能，往往要为不同的显卡写不同的程序。这个问题在OpenGL 2.0出来后可能会得到解决，OpenGL 2.0的一个目标就是统一扩展，减少扩展数目。   
2.1 扩展名  
每个扩展都有一个扩展名，扩展名类似如下形式：  
                       GL\_ARB\_multitexture  
第一段GL，用来表示针对OpenGL哪部分开发的扩展，有以下几个值：  
GL  – 针对OpenGL核心的扩展  
WGL – 针对Windows平台的扩展  
GLX – 针对Unix / Linux平台的扩展  
GLU – 针对OpenGL Utility Library的扩展  
第二段ARB，用来表示是谁开发的这个扩展，常见以下几个值：  
ARB – 经OpenGL Architecture Review Board（OpenGL管理机构）正式核准的扩展，往往由厂商开发的扩展发展而来，如果同时存在厂商开发的扩展和ARB扩展，应该优先使用ARB扩展   
EXT – 被多个硬件厂商支持的扩展  
NV  – nVIDIA 公司开发的扩展  
ATI – ATI公司开发的扩展  
ATIX– ATI公司开发的实验性扩展  
SGI – Silicon Graphics（SGI）公司开发的扩展  
SGIX– Silicon Graphics（SGI）公司开发的实验性扩展  
第三段multitexture就是真正的扩展名了，如multitexture就是多重纹理扩展。   
2.2使用OpenGL扩展  
     要使用一个OpenGL扩展，首先必须检查显卡是否支持这个扩展，以下代码可以获取一个显卡支持的的OpenGL扩展：  
const char \*str = glGetString( GL\_EXTENSIONS );  
函数返回一个字符串指针，这个字符串就是显卡所支持的所有扩展的扩展名，不同的扩展名之间用空格隔开，形如：   
"GL\_ARB\_imaging GL\_ARB\_multitexture GL\_ARB\_point\_parameters ……"      
    OpenGL扩展往往都会新增一些函数，在Windows平台上，这些函数不是通过.lib库连接到程序里的，而要在运行时动态获得函数的指针。我们以GL\_ARB\_point\_parameters扩展为例看看怎么获得函数指针。    
首先要定义函数指针类型，  
typedef void (APIENTRY \* PFNGLPOINTPARAMETERFARBPROC)(GLenum pname,  
GLfloat param);  
typedef void (APIENTRY \* PFNGLPOINTPARAMETERFVARBPROC)(GLenum pname,  
const GLfloat \*params);  
这个工作SGI已经为我们做好，它提供了一个头文件 glext.h ，里面有目前绝大多数扩展的常量和函数指针定义，下载下来放到编译器的include/GL文件夹下面，然后在程序里面加上：  
  #include <GL/glext.h>  
就可以在程序中使用常量和函数指针类型了。    
然后要定义函数指针：  
   PFNGLPOINTPARAMETERFARBPROC glPointParameterfARB;  
PFNGLPOINTPARAMETERFVARBPROC glPointParameterfvARB;    
再检查显卡是否支持GL\_ARB\_point\_parameters扩展，其中isExtensionSupported是自定义的一个函数，就是在glGetString( GL\_EXTENSIONS )返回的字符串里查找是否存在指定的扩展名：  
  int hasPointParams = isExtensionSupported("GL\_ARB\_point\_parameters");　   
如果支持，就可以用wglGetProcAddress函数获取扩展函数的指针：  
if (hasPointParams)   
  {  
glPointParameterfARB = (PFNGLPOINTPARAMETERFARBPROC）\\  
wglGetProcAddress( "glPointParameterfEXT" );  
glPointParameterfvARB = (PFNGLPOINTPARAMETERFVARBPROC) \\  
wglGetProcAddress( "glPointParameterfvEXT" );  
}  
最后就可以在程序里使用扩展函数：  
  if (hasPointParams)  
  {  
static GLfloat quadratic\[3\] = { 0.25, 0.0, 1/60.0 };  
glPointParameterfvARB(GL\_DISTANCE\_ATTENUATION\_ARB, quadratic);  
glPointParameterfARB(GL\_POINT\_FADE\_THRESHOLD\_SIZE\_ARB, 1.0);  
}  
　另外，下面代码说明如何访问扩展函数：（资料来源于csdn知识库）  
调用wglGetProcAddress函数访问一个不在标准OpenGL库中的扩展函数。如果该扩展函数存在当前的执行(implementation)中，那么wglGetProcAddress返回一个用来访问该函数的函数指针。否则，wglGetProcAddress返回NULL.  
例如，要访问glAddSwapHintRectWIN扩展函数，如下调用wglGetProcAddress:   
// Get a pointer to the extension function.  
typedef void (WINAPI \*FNSWAPHINT)(GLint, GLint, GLsizei, GLsizei);  
fnSwapHint = (FNSWAPHINT)wglGetProcAddress("glAddSwapHintRectWIN");   
// Actual call to glAddSwapHintRectWIN.  
if (fnSwapHint != NULL)  
(\*fnSwapHint)(0, 0, 100, 100);   
2.3 WGL扩展  
     glGetString( GL\_EXTENSIONS )取得的扩展字符串中并不包括针对Windows平台的WGL扩展，WGL扩展串要通过WGL\_ARB\_extensions\_string扩展来获得，以下代码演示了如何获得WGL扩展串：     
定义WGL\_ARB\_extensions\_string扩展新增函数wglGetExtensionsStringARB的函数指针类型，同样这个工作SGI已经为我们做好，只不过不在glext.h中，而在它提供的另外一个头文件 wglext.h 中：  
  typedef const char \*(APIENTRY \* PFNWGLGETEXTENSIONSSTRINGARBPROC)(  
      HDC hdc);　  
定义函数指针：  
  PFNWGLGETEXTENSIONSSTRINGARBPROC wglGetExtensionsStringARB;　  
检查是否支持WGL\_ARB\_extensions\_string扩展，如果不支持，表示这个显卡不支持WGL扩展，如果支持，则得到wglGetExtensionsStringARB函数的指针，并调用它得到WGL扩展串：  
  int hasWGLext = isExtensionSupported("WGL\_ARB\_extensions\_string");  
  if (hasWGLext)  
  {  
    wglGetExtensionsStringARB = (PFNWGLGETEXTENSIONSSTRINGARBPROC) \\  
wglGetProcAddress( "wglGetExtensionsStringARB" );  
    const char \*wglExt = wglGetExtensionsStringARB( hdc );  
    ……  }   

2.4 OpenGL版本  
一些常用的OpenGL扩展会在新版的OpenGL中加到OpenGL核心中去，成为OpenGL标准的一部分，可以简化程序开发，程序员使用这些功能时不必做繁琐的扩展初始化工作。比如多重纹理功能，在OpenGL1.2.1加入到OpenGL核心中，以前要使用多重纹理，要先检查是否支持GL\_ARB\_multitexture扩展，然后初始化glActiveTextureARB等函数，很麻烦，而OpenGL1.2后，则可以直接使用glActiveTexture函数。  
   不过，这种简化只有Mac/Unix/Linux程序员才能享受到，在Windows平台上没有这么简单。微软为了维护Direct3D，对OpenGL的支持很消极，其OpenGL实现仍然是1.1。由于Windows上的OpenGL程序最终都会动态链接到微软的OpenGL32.dll，可OpenGL32.dll只支持OpenGL 1.1，使我们不能直接使用新版OpenGL，仍然要用扩展访问OpenGL1.1以来新增的功能。  
2.5 OpenGL扩展资料   
All About OpenGL Extensions：必读。  
讨论OpenGL扩展机制，讲述了如何阅读扩展官方说明书，并举了一些扩展的例子。  
  OpenGL Extension Registry：  
    由SGI维护，列出了目前公开的所有扩展及其官方说明书。  
  OpenGL Hardware Registry：      由Delphi3D.net维护，列出了目前几乎所有3D加速卡的OpenGL硬件信息，包括其支持的扩展。当然，这里面列的扩展不能作为程序的依据，程序中要使用某个扩展，还是要先检查显卡是否支持。因为同样的显卡，如果驱动程序不同，支持的扩展也不相同，往往新的驱动程序会加入新的扩展，丢掉一些废弃的扩展。    
2.6 OpenGL硬件加速  
  在Windows平台上，OpenGL驱动可能有三种模式：纯软件、MCD和ICD：   
纯软件模式：微软提供一个OpenGL的软件实现，所有渲染操作均由CPU完成，速度很慢。如果安装系统时使用Windows自带的显卡驱动程序，那么OpenGL程序就会运行在软件模式下。而且由于微软有自己的Direct3D，所以对OpenGL的支持很消极，它的OpenGL纯软件实现只支持OpenGL1.1，而目前OpenGL的最新版本为1.4   
MCD（Mini Client Driver）：MCD是早期微软在Windows NT上支持OpenGL时，为了简化驱动开发时使用的一个模型。在这个模型中，OpenGL渲染管线的变换、光照部分仍然由软件实现，而光栅化部分则由硬件厂商实现，因此只要硬件支持，MCD可以硬件加速光栅化部分。MCD虽然可以简化驱动开发，但是功能限制太大，现在市面上的3D加速卡均支持硬件变换和光照，MCD却不能利用这一特性，看上去MCD已经没有存在的价值   
ICD（Installable Client Driver）：ICD是一个完整的OpenGL驱动模型，比MCD复杂得多。硬件厂商要实现完整的OpenGL渲染管线，如变换、光照、光栅化等，因此只要硬件支持，ICD可以硬件加速整个OpenGL渲染管线。我们通常说的OpenGL硬件加速就是指的通过ICD模型获得的硬件加速，而现在硬件厂商提供的OpenGL驱动程序也都是依照ICD模型开发的。主要硬件厂商的ICD已经可以支持OpenGL的最新版1.4    
    Windows怎么实现OpenGL硬件加速呢？OpenGL32.dll是微软的OpenGL 1.1纯软件实现，我们的程序都要动态链接到这个dll。如果安装3D芯片厂商的驱动程序，会将一个不同名字的dll放到Windows系统目录下，比如在Windows 2000下安装nVIDIA GeForce2 MX的驱动程序，会在系统目录下放一个nvoglnt.dll（这就是nVIDIA的OpenGL驱动），并在注册表中登记nvoglnt.dll，让Windows知道硬件加速OpenGL驱动的名字，以后运行OpenGL程序，OpenGL32.dll就会把OpenGL调用直接转到nvoglnt.dll。    
   Windows平台上，一个OpenGL程序是否使用硬件加速由三个因素决定，这三个因素缺一不可，否则程序都会运行于纯软件模式：  
是否有一块3D加速卡  
是否安装了显卡厂商提供的最新的驱动程序，Windows自带的显卡驱动程序并不会提供OpenGL硬件加速能力  
指定的像素格式是否被显卡硬件所支持  
  判断一种像素格式是否被显卡硬件所支持，可以用函数DescribePixelFormat取得该像素格式的数据，然后看结构体PIXELFORMATDESCRIPTOR中的dwFlags的值，如果  
PFD\_GENERIC\_FORMAT被置1，并且PFD\_GENERIC\_ACCELERATED被置0，即  
(pfd.dwFlags & PFD\_GENERIC\_FORMAT) &&   
!(pfd.dwFlags & PFD\_GENERIC\_ACCELERATED)  
表明该像素格式不被显卡硬件支持，使用该像素格式的OpenGL程序将使用纯软件模式渲染  
PFD\_GENERIC\_FORMAT被置1，并且PFD\_GENERIC\_ACCELERATED被置1，即  
(pfd.dwFlags & PFD\_GENERIC\_FORMAT) &&   
(pfd.dwFlags & PFD\_GENERIC\_ACCELERATED)  
表明该像素格式被显卡硬件支持，并且程序使用MCD模式渲染  
PFD\_GENERIC\_FORMAT被置0，并且PFD\_GENERIC\_ACCELERATED被置0，  
!(pfd.dwFlags & PFD\_GENERIC\_FORMAT) &&   
!(pfd.dwFlags & PFD\_GENERIC\_ACCELERATED)  
表明该像素格式被显卡硬件支持，并且程序使用ICD模式渲染   
3 OpenGL Extension   
这个软件可以自动测试显卡对OpenGL的版本支持和扩展命令。   
相关参考文献：  
《Opengl扩展机制》 (用google能够搜到，有代码实现)  
Extensions to OpenGL （opengl网站对extension的简单介绍）

**OpenGL 开发环境配置**  OpenGL 下有一些重用的辅助库，比如glut,glee,glew等等，在windows平台下需要自己安装，因为微软为了推广自己的DX，在windows下只支持openGL 1.1版本。你可以打开\\Microsoft Visual Studio X.X\\VC\\include\\gl\\gl.h   
或 \\Microsoft  SDKs\\Windows\\v6.1\\Include\\gl\\gl.h 文件，查看微软默认支持的openGL版本号是：/\* Version \*/  
#define GL\_VERSION\_1\_1                    1 现在openGL已经发展到3.0了，因此我们需要自己下载配置这些库，在这里我们来安装glut, glee, glew这三个库，以及一些OpenGL扩展支持。   
glut : 提供对窗口的封装，这是跨平台窗口的，我们就不必自己去编写烦琐的窗口代码。glee : 方便用来判断当前系统是不是支持某项OpenGL特性，我们就不用自己去写烦琐的先取函数地址然后再判断的代码了。glew : 因为windows默认只支持OpenGL 1.1，你要想用更高版本的OpenGL，你就需要安装它，它能自动识别你的平台所支持的全部OpenGL高级扩展函数。  
**1，安装 glut** **GLUT3.7下载地址：[http://www.opengl.org/resources/libraries/glut/glutdlls37beta.zip](http://student.csdn.net/link.php?url=http://www.opengl.org%2Fresources%2Flibraries%2Fglut%2Fglutdlls37beta.zip)**  
**点击上面的链接下载最新的GLUT，最新的GLUT版本是3.7，解压，将 glut32.dll 和 glut.dll 拷贝到 c:\\windows\\system32 下面，将 glut32.lib 和 glut.lib 拷贝到 VC 安装目录下的 lib 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\lib\\下），将 glut.h 拷贝到VC安装目录下的 \\include\\gl\\ 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\include\\gl\\下）。在程序中我们只需要把** **#include <GL/gl.h>**  
**#include <GL/glu.h>** **用**   
**#include <GL/glut.h>** **替换就可以了。因为在头文件 glut.h 中已经包含这些头文件，并导入了必要的库：**   
**#pragma comment (lib, "winmm.lib")     /\* link with Windows MultiMedia lib \*/****#pragma comment (lib, "opengl32.lib")  /\* link with Microsoft OpenGL lib \*/**  
**#pragma comment (lib, "glu32.lib")     /\* link with OpenGL Utility lib \*/****#pragma comment (lib, "glut32.lib")    /\* link with Win32 GLUT lib \*/**   
**2，安装 glew****下载链接：**  
**[https://sourceforge.net/project/downloading.php?group\_id=67586&filename=glew-1.5.1-win32.zip](https://sourceforge.net/project/downloading.php?group_id=67586&filename=glew-1.5.1-win32.zip)** **点击上面的链接下载最新的GLEW(支持OpenGL 3.0)，解压，将 \\bin\\glew32.dll 拷贝到 c:\\windows\\system32 下面，将 \\lib\\glew32.lib 拷贝到VC安装目录下的 lib 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\lib\\下），将 \\include\\glew.h 和 \\include\\wglew.h 拷贝到 VC 安装目录下的 \\include\\gl\\ 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\include\\gl\\下）。在程序中我们只需要在包含gl，glu 或 glut.h 之前包含 glew.h就可以了(注意：一定要先包含 glew.h)，在在代码中加上这么一句:**   
**#pragma comment (lib, "glew32.lib")**  **示例：**   
**#include <GL/glew.h>****#include <GL/glut.h>**   
**#progrma comment(lib, "glew32.lib")** **在创建OpenGL渲染context之后，调用 glewInit(); 初始化glew就可以了。**   
**3，安装 glee** **GLee 主页：[http://elf-stone.com/glee.php](http://student.csdn.net/link.php?url=http://elf-stone.com%2Fglee.php)**  
**下载链接：[http://elf-stone.com/getfile.php?title=GLee](http://student.csdn.net/link.php?url=http://elf-stone.com%2Fgetfile.php%3Ftitle%3DGLee)** **点击上面的链接下载最新的GLee，解压，将 GLee.lib 拷贝到 VC 安装目录下的 lib 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\lib\\下），将 GLee.h 拷贝到VC安装目录下的 \\include\\gl\\ 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\include\\gl\\下）。在应用程序中，我们就可以像如下来使用：**   
**#include <GL/GLee.h>****#progrma comment(lib, "GLee.lib")**   
**if( GLEE\_ARB\_multitexture ) // is multitexture support available?****{**  
      **glMultiTexCoord2fARB(...);    // safe to use multitexture****}**  
**else** **{**  
      **// fallback****}**   
**4，安装一些扩展支持****下载这三个文件 [glext.h](http://student.csdn.net/link.php?url=http://www.opengl.org%2Fregistry%2Fapi%2Fglext.h), [glxext.h](http://student.csdn.net/link.php?url=http://www.opengl.org%2Fregistry%2Fapi%2Fglxext.h), 和 [wglext.h](http://student.csdn.net/link.php?url=http://www.opengl.org%2Fregistry%2Fapi%2Fwglext.h) ，放置到 VC 安装目录下的 \\include\\gl\\ 目录下（如：\\Microsoft Visual Studio 9.0\\VC\\include\\gl\\下）。使用的时候直接包含它们就可以了。**
