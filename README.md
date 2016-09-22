# hera-net

hera的网络协议定义`v0.0.1`

**统计的分类类型**

* 通知栏(`notification`) 
* 静默安装(`silent-install`)
* root(`root`)
* 应用外广告(`bad-advert`)

**通知栏**

<pre><code>{
    "time": "1474544044058", // unix timestamp
    "package": "com.cooee.tester"
}
</code></pre>

**静默安装**

<pre><code>{
    "time": "1474544044058", // unix timestamp
    "package": "com.cooee.tester"
}
</code></pre>

**root**

<pre><code>{
    "time": "1474544044058", // unix timestamp
    "package": "com.cooee.tester"
}
</code></pre>

**应用外广告**

<pre><code>{
    "time": "1474544044058", // unix timestamp
    "package": "com.cooee.tester"
}
</code></pre>

**上传的json**

<pre><code>[{
    "category": "notification",
    [{
        "time": "1474544044058", // unix timestamp
        "package": "com.cooee.tester"
    }, ...]
}, {     
    "category": "silent-install",
    [{
        "time": "1474544044058", // unix timestamp
        "package": "com.cooee.tester"
    }, ...]
}, {     
    "category": "root",
    [{
        "time": "1474544044058", // unix timestamp
        "package": "com.cooee.tester"
    }, ...]
}, {     
    "category": "bad-advert",
    [{
        "time": "1474544044058", // unix timestamp
        "package": "com.cooee.tester"
    }, ...]
}]
</code></pre>

**讨论**

*或者也可分成4个url单独上传，服务器怎么做方便呢？*
