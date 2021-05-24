# 君凤凰

#### 搜索相关页面
1、搜索页     SearchActivity

2、三级分类   ClassifyThirdActivity

3、店铺内搜索 SearchInShopActivity

其中SearchActivity包含 __搜索店铺__ 和 __搜索商品(ProductsFragment)__

而ProductsFragment 为了复用，从父容器中传递keyword过来搜索商品；复用的地方有：SearchActivity、ClassifyThirdActivity



<del>#### gradle版本要求</del>

<del>Plugin version:3.3.0 - 3.3.2(本项目使用的是3.3.1)</del>

<del>Gradle version:4.10.1+(本项目使用的的是https\://services.gradle.org/distributions/gradle-4.10.1-all.zip)</del>



#### 待优化部分
__1、跳转商品详情的地方，目前是发送事件到MainActivity查询商品类型，然后统一跳转，优化的点在于：可以在列表就知道商品类型，然后直接跳转详情页__

__2、ProductDetailActivity可以优化代码，复用公共Contract（ProdCollectionContract，ShoppingcarContract，SpecContract）__


#### 注
现在的商城有：__普通(秒杀)商城__、__拼团商城__、__积分商城__