Hello and welcome to this blog. Edit the `index.md` file to change this content. All pages on the blog, including this one, use [Markdown](https://guides.github.com/features/mastering-markdown/). You can include images:

![防水](https://github.com/user-attachments/assets/64aba834-43ee-4950-a268-dec7d91c575d)

## this is a AI image for the watch waterproof function

And you can include links, like this [123](https://mp.weixin.qq.com/s/8vpE6jiDAi5EHQAD2B_nlA).


[aaa](https://mp.weixin.qq.com/s/8vpE6jiDAi5EHQAD2B_nlA)Posts will appear after this file. 

Hey, this is a Daniel's Blog


<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>李明的个人主页</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.8/dist/chart.umd.min.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#165DFF',
                        secondary: '#36D399',
                        accent: '#FF6B35',
                        dark: '#1E293B',
                        light: '#F8FAFC'
                    },
                    fontFamily: {
                        inter: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .text-shadow {
                text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            }
            .text-gradient {
                background-clip: text;
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }
            .animate-float {
                animation: float 6s ease-in-out infinite;
            }
            .animate-fade-in {
                animation: fadeIn 0.8s ease-in-out forwards;
            }
            .animate-slide-up {
                animation: slideUp 0.8s ease-out forwards;
            }
            .animate-slide-right {
                animation: slideRight 0.8s ease-out forwards;
            }
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes slideUp {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        @keyframes slideRight {
            from { transform: translateX(-30px); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }
    </style>
</head>
<body class="font-inter bg-light text-dark antialiased">
    <!-- 导航栏 -->
    <header id="navbar" class="fixed w-full top-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-4 py-3 flex items-center justify-between">
            <a href="#hero" class="text-2xl font-bold text-primary flex items-center">
                <span class="mr-2"><i class="fa fa-code"></i></span>
                <span>李明</span>
            </a>
            
            <!-- 桌面导航 -->
            <nav class="hidden md:flex space-x-8">
                <a href="#about" class="text-dark hover:text-primary transition-colors duration-300">关于我</a>
                <a href="#skills" class="text-dark hover:text-primary transition-colors duration-300">技能</a>
                <a href="#projects" class="text-dark hover:text-primary transition-colors duration-300">项目</a>
                <a href="#experience" class="text-dark hover:text-primary transition-colors duration-300">经验</a>
                <a href="#contact" class="text-dark hover:text-primary transition-colors duration-300">联系我</a>
            </nav>
            
            <!-- 移动端菜单按钮 -->
            <button id="menu-toggle" class="md:hidden text-dark focus:outline-none">
                <i class="fa fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- 移动端导航菜单 -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg absolute w-full animate-fade-in">
            <div class="container mx-auto px-4 py-3 flex flex-col space-y-4">
                <a href="#about" class="text-dark hover:text-primary transition-colors duration-300 py-2">关于我</a>
                <a href="#skills" class="text-dark hover:text-primary transition-colors duration-300 py-2">技能</a>
                <a href="#projects" class="text-dark hover:text-primary transition-colors duration-300 py-2">项目</a>
                <a href="#experience" class="text-dark hover:text-primary transition-colors duration-300 py-2">经验</a>
                <a href="#contact" class="text-dark hover:text-primary transition-colors duration-300 py-2">联系我</a>
            </div>
        </div>
    </header>

    <!-- 英雄区域 -->
    <section id="hero" class="min-h-screen flex items-center relative overflow-hidden">
        <div class="absolute inset-0 z-0">
            <div class="absolute inset-0 bg-gradient-to-br from-primary/10 to-secondary/10"></div>
            <div class="absolute top-20 right-20 w-64 h-64 rounded-full bg-primary/20 blur-3xl"></div>
            <div class="absolute bottom-20 left-20 w-80 h-80 rounded-full bg-secondary/20 blur-3xl"></div>
        </div>
        
        <div class="container mx-auto px-4 py-20 relative z-10">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-12 md:mb-0 animate-slide-right opacity-0" style="animation-delay: 0.2s">
                    <h1 class="text-[clamp(2.5rem,5vw,4rem)] font-bold leading-tight text-dark">
                        你好，我是<span class="text-primary">李明</span>
                    </h1>
                    <h2 class="text-[clamp(1.5rem,3vw,2.5rem)] font-semibold text-gray-600 mt-2 mb-6">
                        全栈开发工程师
                    </h2>
                    <p class="text-gray-700 text-lg mb-8 max-w-lg">
                        热衷于创造优雅且高效的解决方案，拥有3年全栈开发经验，擅长前后端技术栈，致力于打造用户体验出色的Web应用。
                    </p>
                    <div class="flex flex-wrap gap-4">
                        <a href="#contact" class="px-8 py-3 bg-primary text-white rounded-full hover:bg-primary/90 transition-all duration-300 shadow-lg hover:shadow-primary/30 hover:-translate-y-1">
                            联系我
                        </a>
                        <a href="#projects" class="px-8 py-3 bg-white text-primary border border-primary rounded-full hover:bg-gray-50 transition-all duration-300 shadow-md hover:shadow-lg hover:-translate-y-1">
                            查看项目
                        </a>
                    </div>
                </div>
                
                <div class="md:w-1/2 relative animate-float">
                    <div class="relative w-64 h-64 md:w-80 md:h-80 mx-auto">
                        <div class="absolute inset-0 bg-gradient-to-br from-primary to-secondary rounded-full blur-xl opacity-50 animate-pulse"></div>
                        <img src="https://picsum.photos/id/1005/400/400" alt="李明的照片" class="absolute inset-4 rounded-full border-4 border-white shadow-2xl object-cover">
                    </div>
                </div>
            </div>
            
            <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
                <a href="#about" class="text-primary/70 hover:text-primary transition-colors duration-300">
                    <i class="fa fa-chevron-down text-2xl"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- 关于我 -->
    <section id="about" class="py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">关于我</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="flex flex-col md:flex-row gap-12 items-center">
                <div class="md:w-1/2 animate-slide-up opacity-0" style="animation-delay: 0.4s">
                    <div class="relative">
                        <img src="https://picsum.photos/id/1070/600/400" alt="工作中的李明" class="rounded-lg shadow-xl w-full">
                        <div class="absolute -bottom-6 -right-6 bg-white p-4 rounded-lg shadow-lg">
                            <div class="flex items-center gap-3">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary">
                                    <i class="fa fa-code text-xl"></i>
                                </div>
                                <div>
                                    <p class="text-sm text-gray-500">3年工作经验</p>
                                    <p class="font-semibold">全栈开发</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2 animate-slide-up opacity-0" style="animation-delay: 0.6s">
                    <h3 class="text-2xl font-semibold mb-4">你好，我是李明，全栈开发工程师</h3>
                    <p class="text-gray-700 mb-6">
                        我毕业于北京大学计算机科学专业，拥有3年Web开发经验。目前在一家科技公司担任全栈开发工程师，负责设计和实现用户友好的Web应用程序。
                    </p>
                    <p class="text-gray-700 mb-8">
                        我热衷于学习新技术，不断提升自己的技能，致力于创建高质量的软件解决方案。我的开发理念是将技术与用户体验完美结合，创造出既实用又美观的产品。
                    </p>
                    
                    <div class="grid grid-cols-2 gap-6 mb-8">
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary">
                                <i class="fa fa-birthday-cake"></i>
                            </div>
                            <div>
                                <p class="text-sm text-gray-500">出生日期</p>
                                <p>1995年3月12日</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary">
                                <i class="fa fa-envelope"></i>
                            </div>
                            <div>
                                <p class="text-sm text-gray-500">电子邮箱</p>
                                <p>liming@example.com</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary">
                                <i class="fa fa-phone"></i>
                            </div>
                            <div>
                                <p class="text-sm text-gray-500">电话</p>
                                <p>+86 138 1234 5678</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center gap-3">
                            <div class="w-10 h-10 bg-primary/10 rounded-full flex items-center justify-center text-primary">
                                <i class="fa fa-map-marker"></i>
                            </div>
                            <div>
                                <p class="text-sm text-gray-500">所在地</p>
                                <p>北京市海淀区</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-4">
                        <a href="#" class="px-6 py-2 bg-primary text-white rounded-full hover:bg-primary/90 transition-all duration-300 shadow-md hover:shadow-lg">
                            <i class="fa fa-download mr-2"></i>下载简历
                        </a>
                        <a href="#contact" class="px-6 py-2 bg-white text-primary border border-primary rounded-full hover:bg-gray-50 transition-all duration-300 shadow-sm hover:shadow-md">
                            <i class="fa fa-envelope mr-2"></i>联系我
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 技能 -->
    <section id="skills" class="py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">我的技能</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
                    以下是我掌握的技术栈和专业技能，不断学习和提升中...
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
                <div class="bg-white rounded-xl shadow-lg p-8 animate-slide-up opacity-0" style="animation-delay: 0.4s">
                    <h3 class="text-xl font-semibold mb-6 flex items-center">
                        <i class="fa fa-code text-primary mr-3"></i>
                        技术技能
                    </h3>
                    
                    <div class="space-y-6">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">前端开发</span>
                                <span>90%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-primary rounded-full" style="width: 90%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">后端开发</span>
                                <span>85%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-primary rounded-full" style="width: 85%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">数据库设计</span>
                                <span>80%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-primary rounded-full" style="width: 80%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">移动应用开发</span>
                                <span>75%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-primary rounded-full" style="width: 75%"></div>
                            </div>
                        </div>
                        
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="font-medium">DevOps</span>
                                <span>70%</span>
                            </div>
                            <div class="h-2 bg-gray-200 rounded-full overflow-hidden">
                                <div class="h-full bg-primary rounded-full" style="width: 70%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-xl shadow-lg p-8 animate-slide-up opacity-0" style="animation-delay: 0.6s">
                    <h3 class="text-xl font-semibold mb-6 flex items-center">
                        <i class="fa fa-laptop text-primary mr-3"></i>
                        专业知识
                    </h3>
                    
                    <div class="grid grid-cols-2 gap-4">
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-html5 text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">HTML5 & CSS3</h4>
                            <p class="text-sm text-gray-600">精通响应式设计和现代布局技术</p>
                        </div>
                        
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-js text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">JavaScript</h4>
                            <p class="text-sm text-gray-600">熟悉ES6+、异步编程和函数式编程</p>
                        </div>
                        
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-database text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">数据库</h4>
                            <p class="text-sm text-gray-600">熟练掌握MySQL、PostgreSQL和MongoDB</p>
                        </div>
                        
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-cubes text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">框架与库</h4>
                            <p class="text-sm text-gray-600">React、Vue、Node.js、Express等</p>
                        </div>
                        
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-cloud text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">云计算</h4>
                            <p class="text-sm text-gray-600">AWS、阿里云、Docker和Kubernetes</p>
                        </div>
                        
                        <div class="bg-gray-50 p-4 rounded-lg hover:shadow-md transition-all duration-300 hover:-translate-y-1">
                            <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary mb-3">
                                <i class="fa fa-git text-xl"></i>
                            </div>
                            <h4 class="font-medium mb-1">版本控制</h4>
                            <p class="text-sm text-gray-600">Git工作流和团队协作</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-16 bg-white rounded-xl shadow-lg p-8 animate-slide-up opacity-0" style="animation-delay: 0.8s">
                <h3 class="text-xl font-semibold mb-6 flex items-center">
                    <i class="fa fa-pie-chart text-primary mr-3"></i>
                    技能分布
                </h3>
                
                <div class="h-80">
                    <canvas id="skillsChart"></canvas>
                </div>
            </div>
        </div>
    </section>

    <!-- 项目展示 -->
    <section id="projects" class="py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">我的项目</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
                    以下是我参与过的一些项目，涵盖Web应用、移动应用和系统开发
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- 项目1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.4s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/0/600/400" alt="电商平台项目" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">React</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">Node.js</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">现代电商平台</h3>
                        <p class="text-gray-600 mb-4">
                            一个功能完整的电商平台，支持商品浏览、购物车、支付流程和用户管理等功能。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2024</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 3人团队</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- 项目2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.5s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/180/600/400" alt="数据分析仪表盘" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">Vue</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">D3.js</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">数据分析仪表盘</h3>
                        <p class="text-gray-600 mb-4">
                            一个数据可视化仪表盘，支持多维度数据分析、图表展示和数据导出功能。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2024</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 2人团队</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- 项目3 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.6s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/160/600/400" alt="移动应用" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">React Native</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">Firebase</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">健康追踪应用</h3>
                        <p class="text-gray-600 mb-4">
                            一款跨平台健康追踪应用，支持运动记录、饮食管理和健康数据分析。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2023</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 4人团队</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- 项目4 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.7s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/119/600/400" alt="企业管理系统" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">Angular</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">.NET</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">企业资源管理系统</h3>
                        <p class="text-gray-600 mb-4">
                            一套完整的企业资源管理系统，包括人力资源、财务管理和项目管理模块。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2023</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 5人团队</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- 项目5 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.8s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/1/600/400" alt="社交媒体应用" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">Vue</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">GraphQL</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">社交分享平台</h3>
                        <p class="text-gray-600 mb-4">
                            一个轻量级社交分享平台，支持内容发布、互动评论和用户关注等功能。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2022</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 3人团队</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- 项目6 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.9s">
                    <div class="relative h-60 overflow-hidden">
                        <img src="https://picsum.photos/id/111/600/400" alt="开源项目" class="w-full h-full object-cover transition-transform duration-500 hover:scale-110">
                        <div class="absolute inset-0 bg-gradient-to-t from-black/70 to-transparent flex items-end">
                            <div class="p-6">
                                <span class="px-3 py-1 bg-primary text-white text-xs rounded-full">Node.js</span>
                                <span class="px-3 py-1 bg-secondary text-white text-xs rounded-full ml-2">MongoDB</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">开源博客平台</h3>
                        <p class="text-gray-600 mb-4">
                            一个基于Node.js的开源博客平台，支持Markdown编辑、评论系统和主题定制。
                        </p>
                        <div class="flex justify-between items-center">
                            <div class="flex space-x-2">
                                <span class="text-xs text-gray-500"><i class="fa fa-calendar mr-1"></i> 2022</span>
                                <span class="text-xs text-gray-500"><i class="fa fa-users mr-1"></i> 个人项目</span>
                            </div>
                            <a href="#" class="text-primary hover:text-primary/80 transition-colors duration-300">
                                查看详情 <i class="fa fa-arrow-right ml-1"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-flex items-center px-8 py-3 bg-primary text-white rounded-full hover:bg-primary/90 transition-all duration-300 shadow-lg hover:shadow-primary/30 hover:-translate-y-1">
                    查看更多项目 <i class="fa fa-arrow-right ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- 工作经验 -->
    <section id="experience" class="py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">工作经验</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
                    以下是我的职业经历和相关职责
                </p>
            </div>
            
            <div class="relative">
                <!-- 时间线 -->
                <div class="absolute left-0 md:left-1/2 top-0 bottom-0 w-1 bg-primary/20 transform md:-translate-x-1/2"></div>
                
                <!-- 经验1 -->
                <div class="relative mb-12 md:mb-24 animate-slide-right opacity-0" style="animation-delay: 0.4s">
                    <div class="md:w-1/2 md:pr-12 md:text-right">
                        <div class="bg-white p-6 rounded-xl shadow-lg">
                            <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-3">
                                2023年至今
                            </span>
                            <h3 class="text-xl font-semibold mb-2">高级全栈开发工程师</h3>
                            <p class="text-gray-500 mb-3">科技有限公司</p>
                            <p class="text-gray-600">
                                负责公司核心产品的架构设计和技术实现，带领团队开发新功能和优化现有系统。主导前端技术栈升级，提高了开发效率和用户体验。
                            </p>
                            <ul class="mt-4 space-y-2 text-gray-600">
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>设计和实现微服务架构，提高系统可扩展性和可靠性</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>优化前端性能，页面加载速度提升了40%</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>建立代码规范和开发流程，提高团队协作效率</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="absolute left-0 md:left-1/2 top-8 w-4 h-4 bg-primary rounded-full transform md:-translate-x-1/2 border-4 border-white shadow-md"></div>
                </div>
                
                <!-- 经验2 -->
                <div class="relative mb-12 md:mb-24 animate-slide-left opacity-0 md:ml-auto md:text-left" style="animation-delay: 0.6s">
                    <div class="md:w-1/2 md:pl-12 md:ml-auto">
                        <div class="bg-white p-6 rounded-xl shadow-lg">
                            <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-3">
                                2021-2023年
                            </span>
                            <h3 class="text-xl font-semibold mb-2">全栈开发工程师</h3>
                            <p class="text-gray-500 mb-3">互联网公司</p>
                            <p class="text-gray-600">
                                参与公司多个Web应用的开发和维护，负责前后端开发和数据库设计。与产品和设计团队紧密合作，实现用户需求并优化用户体验。
                            </p>
                            <ul class="mt-4 space-y-2 text-gray-600">
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>开发和维护电商平台，支持数万用户同时在线购物</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>设计和实现API接口，支持移动端和第三方集成</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>参与系统性能优化，减少响应时间和服务器负载</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="absolute left-0 md:left-1/2 top-8 w-4 h-4 bg-primary rounded-full transform md:-translate-x-1/2 border-4 border-white shadow-md"></div>
                </div>
                
                <!-- 经验3 -->
                <div class="relative animate-slide-right opacity-0" style="animation-delay: 0.8s">
                    <div class="md:w-1/2 md:pr-12 md:text-right">
                        <div class="bg-white p-6 rounded-xl shadow-lg">
                            <span class="inline-block px-3 py-1 bg-primary/10 text-primary text-sm font-medium rounded-full mb-3">
                                2019-2021年
                            </span>
                            <h3 class="text-xl font-semibold mb-2">前端开发工程师</h3>
                            <p class="text-gray-500 mb-3">软件公司</p>
                            <p class="text-gray-600">
                                专注于Web前端开发，负责公司产品的用户界面设计和实现。使用现代前端技术栈构建响应式、交互友好的用户界面。
                            </p>
                            <ul class="mt-4 space-y-2 text-gray-600">
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>使用React和Vue开发企业级应用界面</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>优化前端资源加载，提高页面性能</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fa fa-check text-secondary mt-1 mr-2"></i>
                                    <span>与后端团队协作，设计和实现API接口</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="absolute left-0 md:left-1/2 top-8 w-4 h-4 bg-primary rounded-full transform md:-translate-x-1/2 border-4 border-white shadow-md"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- 教育背景 -->
    <section id="education" class="py-24 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">教育背景</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- 教育1 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.4s">
                    <div class="bg-primary/10 p-6">
                        <h3 class="text-xl font-semibold text-primary">北京大学</h3>
                        <p class="text-gray-600">计算机科学与技术</p>
                        <p class="text-gray-500 text-sm mt-2">2015-2019年 | 本科</p>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            主修计算机科学与技术，专注于软件开发和人工智能方向。获得优秀毕业生称号，GPA 3.8/4.0。
                        </p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">数据结构</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">算法设计</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">计算机网络</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">操作系统</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">数据库系统</span>
                        </div>
                    </div>
                </div>
                
                <!-- 教育2 -->
                <div class="bg-white rounded-xl overflow-hidden shadow-lg hover:shadow-xl transition-all duration-300 hover:-translate-y-2 animate-slide-up opacity-0" style="animation-delay: 0.6s">
                    <div class="bg-primary/10 p-6">
                        <h3 class="text-xl font-semibold text-primary">清华大学</h3>
                        <p class="text-gray-600">软件工程</p>
                        <p class="text-gray-500 text-sm mt-2">2019-2021年 | 硕士</p>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            攻读软件工程专业硕士学位，研究方向为Web应用开发和云计算。发表2篇学术论文，参与多个科研项目。
                        </p>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">高级编程</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">软件开发方法</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">云计算</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">人工智能</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-700 text-xs rounded-full">分布式系统</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 联系我 -->
    <section id="contact" class="py-24 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16 animate-fade-in opacity-0" style="animation-delay: 0.3s">
                <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold text-dark mb-4">联系我</h2>
                <div class="w-20 h-1 bg-primary mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">
                    无论你有任何问题或合作机会，都可以通过以下方式联系我
                </p>
            </div>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <div class="animate-slide-up opacity-0" style="animation-delay: 0.4s">
                    <div class="bg-white rounded-xl shadow-lg p-8 h-full">
                        <h3 class="text-xl font-semibold mb-6">发送消息</h3>
                        
                        <form id="contact-form" class="space-y-6">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                <div>
                                    <label for="name" class="block text-sm font-medium text-gray-700 mb-1">姓名</label>
                                    <input type="text" id="name" name="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-all duration-300" placeholder="请输入您的姓名" required>
                                </div>
                                
                                <div>
                                    <label for="email" class="block text-sm font-medium text-gray-700 mb-1">电子邮箱</label>
                                    <input type="email" id="email" name="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-all duration-300" placeholder="请输入您的电子邮箱" required>
                                </div>
                            </div>
                            
                            <div>
                                <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">主题</label>
                                <input type="text" id="subject" name="subject" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-all duration-300" placeholder="请输入消息主题" required>
                            </div>
                            
                            <div>
                                <label for="message" class="block text-sm font-medium text-gray-700 mb-1">消息内容</label>
                                <textarea id="message" name="message" rows="5" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary focus:border-primary transition-all duration-300" placeholder="请输入您的消息内容" required></textarea>
                            </div>
                            
                            <button type="submit" class="w-full px-6 py-3 bg-primary text-white rounded-lg hover:bg-primary/90 transition-all duration-300 shadow-md hover:shadow-lg hover:-translate-y-1">
                                发送消息 <i class="fa fa-paper-plane ml-2"></i>
                            </button>
                        </form>
                    </div>
                </div>
                
                <div class="animate-slide-up opacity-0" style="animation-delay: 0.6s">
                    <div class="bg-white rounded-xl shadow-lg p-8 mb-8">
                        <h3 class="text-xl font-semibold mb-6">联系方式</h3>
                        
                        <div class="space-y-6">
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary shrink-0">
                                    <i class="fa fa-map-marker text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-medium mb-1">地址</h4>
                                    <p class="text-gray-600">北京市海淀区中关村大街1号</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary shrink-0">
                                    <i class="fa fa-envelope text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-medium mb-1">电子邮箱</h4>
                                    <p class="text-gray-600">liming@example.com</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary shrink-0">
                                    <i class="fa fa-phone text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-medium mb-1">电话</h4>
                                    <p class="text-gray-600">+86 138 1234 5678</p>
                                </div>
                            </div>
                            
                            <div class="flex items-start">
                                <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center text-primary shrink-0">
                                    <i class="fa fa-clock-o text-xl"></i>
                                </div>
                                <div class="ml-4">
                                    <h4 class="font-medium mb-1">工作时间</h4>
                                    <p class="text-gray-600">周一至周五: 9:00 - 18:00</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-white rounded-xl shadow-lg p-8">
                        <h3 class="text-xl font-semibold mb-6">社交媒体</h3>
                        
                        <div class="grid grid-cols-2 gap-4">
                            <a href="#" class="flex items-center p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-all duration-300">
                                <div class="w-10 h-10 bg-blue-500 rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fa fa-github"></i>
                                </div>
                                <div>
                                    <h4 class="font-medium">GitHub</h4>
                                    <p class="text-gray-600 text-sm">@limingdev</p>
                                </div>
                            </a>
                            
                            <a href="#" class="flex items-center p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-all duration-300">
                                <div class="w-10 h-10 bg-blue-600 rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fa fa-linkedin"></i>
                                </div>
                                <div>
                                    <h4 class="font-medium">LinkedIn</h4>
                                    <p class="text-gray-600 text-sm">李明</p>
                                </div>
                            </a>
                            
                            <a href="#" class="flex items-center p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-all duration-300">
                                <div class="w-10 h-10 bg-red-500 rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fa fa-twitter"></i>
                                </div>
                                <div>
                                    <h4 class="font-medium">Twitter</h4>
                                    <p class="text-gray-600 text-sm">@liming_dev</p>
                                </div>
                            </a>
                            
                            <a href="#" class="flex items-center p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-all duration-300">
                                <div class="w-10 h-10 bg-red-600 rounded-full flex items-center justify-center text-white mr-4">
                                    <i class="fa fa-weixin"></i>
                                </div>
                                <div>
                                    <h4 class="font-medium">微信</h4>
                                    <p class="text-gray-600 text-sm">liming_tech</p>
                                </div>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="bg-dark text-white py-12">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-6 md:mb-0">
                    <a href="#hero" class="text-2xl font-bold flex items-center">
                        <span class="mr-2"><i class="fa fa-code"></i></span>
                        <span>李明</span>
                    </a>
                    <p class="text-gray-400 mt-2">全栈开发工程师</p>
                </div>
                
                <div class="flex space-x-6 mb-6 md:mb-0">
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">
                        <i class="fa fa-github text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">
                        <i class="fa fa-linkedin text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">
                        <i class="fa fa-twitter text-xl"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">
                        <i class="fa fa-weixin text-xl"></i>
                    </a>
                </div>
                
                <div>
                    <p class="text-gray-400">© 2025 李明. 保留所有权利.</p>
                </div>
            </div>
        </div>
    </footer>

    <!-- 返回顶部按钮 -->
    <button id="back-to-top" class="fixed bottom-6 right-6 w-12 h-12 bg-primary text-white rounded-full flex items-center justify-center shadow-lg hover:bg-primary/90 transition-all duration-300 opacity-0 invisible">
        <i class="fa fa-chevron-up"></i>
    </button>

    <!-- JavaScript -->
    <script>
        // 导航栏滚动效果
        const navbar = document.getElementById('navbar');
        const backToTopBtn = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', function() {
            if (window.scrollY > 50) {
                navbar.classList.add('bg-white', 'shadow-md');
                navbar.classList.remove('py-3');
                navbar.classList.add('py-2');
                
                backToTopBtn.classList.remove('opacity-0', 'invisible');
                backToTopBtn.classList.add('opacity-100');
            } else {
                navbar.classList.remove('bg-white', 'shadow-md');
                navbar.classList.remove('py-2');
                navbar.classList.add('py-3');
                
                backToTopBtn.classList.add('opacity-0', 'invisible');
                backToTopBtn.classList.remove('opacity-100');
            }
        });
        
        // 移动端菜单切换
        const menuToggle = document.getElementById('menu-toggle');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuToggle.addEventListener('click', function() {
            mobileMenu.classList.toggle('hidden');
        });
        
        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // 关闭移动端菜单
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
        
        // 返回顶部按钮
        backToTopBtn.addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // 技能图表
        window.addEventListener('load', function() {
            const ctx = document.getElementById('skillsChart').getContext('2d');
            
            new Chart(ctx, {
                type: 'radar',
                data: {
                    labels: ['前端开发', '后端开发', '数据库设计', '移动应用', 'DevOps', 'UI/UX设计', '项目管理'],
                    datasets: [{
                        label: '技能水平',
                        data: [90, 85, 80, 75, 70, 65, 75],
                        backgroundColor: 'rgba(22, 93, 255, 0.2)',
                        borderColor: 'rgba(22, 93, 255, 1)',
                        pointBackgroundColor: 'rgba(22, 93, 255, 1)',
                        pointBorderColor: '#fff',
                        pointHoverBackgroundColor: '#fff',
                        pointHoverBorderColor: 'rgba(22, 93, 255, 1)'
                    }]
                },
                options: {
                    scales: {
                        r: {
                            angleLines: {
                                display: true
                            },
                            suggestedMin: 0,
                            suggestedMax: 100
                        }
                    }
                }
            });
        });
        
        // 表单提交
        const contactForm = document.getElementById('contact-form');
        
        contactForm.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // 这里可以添加表单验证和提交逻辑
            alert('感谢您的留言！我会尽快回复您。');
            contactForm.reset();
        });
        
        // 动画效果
        function animateOnScroll() {
            const elements = document.querySelectorAll('.animate-fade-in, .animate-slide-up, .animate-slide-right, .animate-slide-left');
            
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const windowHeight = window.innerHeight;
                
                if (elementPosition < windowHeight - 100) {
                    element.style.opacity = '1';
                    element.style.transform = 'translateY(0)';
                }
            });
        }
        
        // 初始加载时执行一次
        window.addEventListener('load', animateOnScroll);
        
        // 滚动时执行
        window.addEventListener('scroll', animateOnScroll);
    </script>
</body>
</html>
    
