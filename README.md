<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>家教资料中心</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#3B82F6',
                        secondary: '#10B981',
                        accent: '#F59E0B',
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .text-shadow {
                text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            }
            .card-hover {
                transition: all 0.3s ease;
            }
            .card-hover:hover {
                transform: translateY(-5px);
            }
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- 导航栏 -->
    <nav class="bg-white shadow-md fixed w-full top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <i class="fa fa-graduation-cap text-primary text-2xl"></i>
                <span class="font-bold text-xl text-gray-800">优学家教资料中心</span>
            </div>
            <div class="hidden md:flex items-center space-x-6">
                <a href="#" class="text-gray-600 hover:text-primary transition">首页</a>
                <a href="#" class="text-gray-600 hover:text-primary transition">小学资料</a>
                <a href="#" class="text-gray-600 hover:text-primary transition">中学资料</a>
                <a href="#" class="text-gray-600 hover:text-primary transition">联系我们</a>
            </div>
            <button class="md:hidden text-gray-600">
                <i class="fa fa-bars text-xl"></i>
            </button>
        </div>
    </nav>

    <!-- 头部横幅 -->
    <header class="pt-20 pb-10 bg-gradient-to-r from-primary to-blue-700 text-white">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-[clamp(1.8rem,5vw,3rem)] font-bold mb-4 text-shadow">优质家教资料免费领取</h1>
            <p class="text-lg md:text-xl max-w-2xl mx-auto opacity-90">精选小学到高中各学科学习资料，助力孩子高效学习</p>
            <div class="mt-8">
                <button class="bg-white text-primary px-6 py-3 rounded-full font-medium shadow-lg hover:shadow-xl transition transform hover:-translate-y-1">
                    <i class="fa fa-download mr-2"></i>立即领取
                </button>
            </div>
        </div>
    </header>

    <!-- 资料分类 -->
    <section class="py-12 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-10 text-gray-800">资料分类</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- 小学资料 -->
                <div class="bg-blue-50 rounded-xl p-6 shadow-md card-hover">
                    <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa fa-child text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2 text-gray-800">小学资料</h3>
                    <p class="text-gray-600 mb-4">包含小学语文、数学、英语等学科的同步练习、单元测试和知识点总结</p>
                    <a href="#" class="text-primary font-medium flex items-center">
                        查看全部 <i class="fa fa-arrow-right ml-2"></i>
                    </a>
                </div>
                
                <!-- 初中资料 -->
                <div class="bg-green-50 rounded-xl p-6 shadow-md card-hover">
                    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa fa-book text-secondary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2 text-gray-800">初中资料</h3>
                    <p class="text-gray-600 mb-4">包含初中各学科同步辅导、中考真题、专题训练和学习方法指导</p>
                    <a href="#" class="text-secondary font-medium flex items-center">
                        查看全部 <i class="fa fa-arrow-right ml-2"></i>
                    </a>
                </div>
                
                <!-- 高中资料 -->
                <div class="bg-orange-50 rounded-xl p-6 shadow-md card-hover">
                    <div class="w-16 h-16 bg-orange-100 rounded-full flex items-center justify-center mb-4">
                        <i class="fa fa-graduation-cap text-accent text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2 text-gray-800">高中资料</h3>
                    <p class="text-gray-600 mb-4">包含高中各学科重难点解析、高考模拟题、学霸笔记和备考策略</p>
                    <a href="#" class="text-accent font-medium flex items-center">
                        查看全部 <i class="fa fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- 热门资料 -->
    <section class="py-12 bg-gray-50">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-10 text-gray-800">热门资料</h2>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- 资料卡片1 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md card-hover">
                    <div class="h-40 bg-blue-100 flex items-center justify-center">
                        <i class="fa fa-file-pdf-o text-5xl text-primary/70"></i>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold text-gray-800 mb-2">小学数学公式大全</h3>
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <i class="fa fa-eye mr-1"></i> 2.3k次查看
                            <span class="mx-2">•</span>
                            <i class="fa fa-download mr-1"></i> 1.8k次下载
                        </div>
                        <button class="w-full bg-primary text-white py-2 rounded hover:bg-primary/90 transition">
                            免费领取
                        </button>
                    </div>
                </div>
                
                <!-- 资料卡片2 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md card-hover">
                    <div class="h-40 bg-green-100 flex items-center justify-center">
                        <i class="fa fa-file-word-o text-5xl text-secondary/70"></i>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold text-gray-800 mb-2">初中英语语法手册</h3>
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <i class="fa fa-eye mr-1"></i> 1.9k次查看
                            <span class="mx-2">•</span>
                            <i class="fa fa-download mr-1"></i> 1.5k次下载
                        </div>
                        <button class="w-full bg-secondary text-white py-2 rounded hover:bg-secondary/90 transition">
                            免费领取
                        </button>
                    </div>
                </div>
                
                <!-- 资料卡片3 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md card-hover">
                    <div class="h-40 bg-orange-100 flex items-center justify-center">
                        <i class="fa fa-file-excel-o text-5xl text-accent/70"></i>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold text-gray-800 mb-2">高中物理必刷题</h3>
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <i class="fa fa-eye mr-1"></i> 1.7k次查看
                            <span class="mx-2">•</span>
                            <i class="fa fa-download mr-1"></i> 1.2k次下载
                        </div>
                        <button class="w-full bg-accent text-white py-2 rounded hover:bg-accent/90 transition">
                            免费领取
                        </button>
                    </div>
                </div>
                
                <!-- 资料卡片4 -->
                <div class="bg-white rounded-lg overflow-hidden shadow-md card-hover">
                    <div class="h-40 bg-purple-100 flex items-center justify-center">
                        <i class="fa fa-file-powerpoint-o text-5xl text-purple-500/70"></i>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold text-gray-800 mb-2">作文写作技巧</h3>
                        <div class="flex items-center text-sm text-gray-500 mb-3">
                            <i class="fa fa-eye mr-1"></i> 2.1k次查看
                            <span class="mx-2">•</span>
                            <i class="fa fa-download mr-1"></i> 1.6k次下载
                        </div>
                        <button class="w-full bg-purple-500 text-white py-2 rounded hover:bg-purple-600 transition">
                            免费领取
                        </button>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-10">
                <a href="#" class="inline-block border-2 border-primary text-primary px-6 py-2 rounded-full font-medium hover:bg-primary hover:text-white transition">
                    查看更多资料
                </a>
            </div>
        </div>
    </section>

    <!-- 领取方式 -->
    <section class="py-12 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-10 text-gray-800">资料领取方式</h2>
            
            <div class="max-w-3xl mx-auto">
                <div class="flex flex-col md:flex-row mb-8">
                    <div class="md:w-1/4 flex justify-center md:justify-start mb-4 md:mb-0">
                        <div class="w-12 h-12 bg-primary text-white rounded-full flex items-center justify-center font-bold text-xl">1</div>
                    </div>
                    <div class="md:w-3/4">
                        <h3 class="text-xl font-semibold mb-2 text-gray-800">关注我们的公众号</h3>
                        <p class="text-gray-600">扫描下方二维码或搜索公众号名称关注，获取更多优质教育资源</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row mb-8">
                    <div class="md:w-1/4 flex justify-center md:justify-start mb-4 md:mb-0">
                        <div class="w-12 h-12 bg-primary text-white rounded-full flex items-center justify-center font-bold text-xl">2</div>
                    </div>
                    <div class="md:w-3/4">
                        <h3 class="text-xl font-semibold mb-2 text-gray-800">回复关键词</h3>
                        <p class="text-gray-600">在公众号对话框中回复资料对应的关键词，获取下载链接</p>
                    </div>
                </div>
                
                <div class="flex flex-col md:flex-row">
                    <div class="md:w-1/4 flex justify-center md:justify-start mb-4 md:mb-0">
                        <div class="w-12 h-12 bg-primary text-white rounded-full flex items-center justify-center font-bold text-xl">3</div>
                    </div>
                    <div class="md:w-3/4">
                        <h3 class="text-xl font-semibold mb-2 text-gray-800">下载使用</h3>
                        <p class="text-gray-600">点击链接下载资料，打印后即可使用，也可在电子设备上直接查看</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 公众号二维码 -->
    <section class="py-12 bg-gray-50">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-2xl md:text-3xl font-bold mb-6 text-gray-800">关注公众号，获取更多资料</h2>
            <p class="text-gray-600 mb-8 max-w-xl mx-auto">扫码关注我们的公众号，第一时间获取最新教育资源和家教信息</p>
            
            <div class="inline-block bg-white p-4 rounded-lg shadow-md">
                <div class="w-48 h-48 bg-gray-200 mx-auto flex items-center justify-center">
                    <!-- 这里放置公众号二维码 -->
                    <i class="fa fa-qrcode text-6xl text-gray-400"></i>
                </div>
                <p class="mt-4 font-medium text-gray-800">优学家教联盟</p>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer class="bg-gray-800 text-white py-10">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-xl font-semibold mb-4">关于我们</h3>
                    <p class="text-gray-400">我们是由大学生组成的家教团队，致力于为中小学生提供优质的家教服务和学习资料</p>
                </div>
                
                <div>
                    <h3 class="text-xl font-semibold mb-4">联系方式</h3>
                    <p class="text-gray-400 mb-2"><i class="fa fa-weixin mr-2"></i> 客服微信：xxx123</p>
                    <p class="text-gray-400"><i class="fa fa-phone mr-2"></i> 联系电话：138-xxxx-xxxx</p>
                </div>
                
                <div>
                    <h3 class="text-xl font-semibold mb-4">快速链接</h3>
                    <ul class="text-gray-400 space-y-2">
                        <li><a href="#" class="hover:text-white transition">家教介绍</a></li>
                        <li><a href="#" class="hover:text-white transition">老师招募</a></li>
                        <li><a href="#" class="hover:text-white transition">常见问题</a></li>
                        <li><a href="#" class="hover:text-white transition">资料反馈</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-500">
                <p>© 2023 优学家教联盟 版权所有</p>
            </div>
        </div>
    </footer>

    <script>
        // 简单的交互效果
        document.addEventListener('DOMContentLoaded', function() {
            // 滚动时导航栏样式变化
            window.addEventListener('scroll', function() {
                const nav = document.querySelector('nav');
                if (window.scrollY > 50) {
                    nav.classList.add('py-2');
                    nav.classList.remove('py-3');
                } else {
                    nav.classList.add('py-3');
                    nav.classList.remove('py-2');
                }
            });
            
            // 领取按钮点击效果
            const downloadButtons = document.querySelectorAll('button');
            downloadButtons.forEach(button => {
                if (button.textContent.includes('领取')) {
                    button.addEventListener('click', function() {
                        alert('请在公众号内回复关键词 "资料领取" 获取下载链接');
                    });
                }
            });
        });
    </script>
</body>
</html>
