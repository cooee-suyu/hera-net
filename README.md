# hera-net

hera的网络协议定义`v0.0.3`

## 统计的分类类型

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

## 上传统计信息

**上传的json**

<pre><code>{
    "device": {object} // the device object
    "data": [{
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
}
</code></pre>

## 拉取配置

**上传的json**

<pre><code>{
    "device": {object} // the device object
}
</code></pre>

**下行的json**

<pre><code>{
    "data": [{
        "category": "notification",
        "list-type": "black" or "white"
        [{
            "package": "com.cooee.tester"
        }, ...]
    }, {     
        "category": "silent-install",
        "list-type": "black" or "white"
        [{
            "package": "com.cooee.tester"
        }, ...]
    }, {     
        "category": "root",
        "list-type": "black" or "white"
        [{
            "package": "com.cooee.tester"
        }, ...]
    }, {     
        "category": "bad-advert",
        "list-type": "black" or "white"
        [{
            "package": "com.cooee.tester"
        }, ...]
    }]
}
</code></pre>

**讨论**

*请帮忙按照通用标准来定义device object*

*统计信息的上传可合并也可分开，请根据服务器需求来选择*
