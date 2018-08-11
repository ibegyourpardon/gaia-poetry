# gaia-poetry


###简介###
盖亚·古诗词 API 是一个可以随机返回一首古诗词名句的接口。

提供两种返回方式。

###API地址

随机返回一句古诗词
https://gaiaaaa.com/api/poetry/random

###请求方式：###
GET
###请求参数：###
无

###返回结果（JSON）###
<pre>
<code>
{
code: 200,
data: {
id: 106192,
title: "訓蒙絕句 吾無隠乎爾",
yunlv_rule: "仄仄平平仄仄平，平平仄仄仄平平。|平平仄仄平平仄，仄仄平平仄仄平。",
author_id: 8325,
content: "聖道雖云妙莫窺，初非恍惚與希夷。|分明說在吾行處，後學無於行外思。",
dynasty: "S",
author: "朱熹",
dy: "宋"
}
}
</code></pre>


###API地址

根据关键字返回一句古诗词
https://gaiaaaa.com/api/poetry/find

###请求方式：###
GET
###请求参数：###
?key_word=

###返回结果（JSON）###
?key_word=我
<pre>
<code>
{
code: 200,
data: {
title: "己亥季秋至凈居思大智者道場因瞻二士相三日會天大雨不得探險絕而以詩記之 其四",
author: "李彌遜",
content: "白霧蒼烟暗九秋，殷牀金吼抱山樓。|爲霖未必渾三日，似有閑雲伴我留。",
dynasty: "S",
dy: "宋"
}
}
</code></pre>

后台 Laravel ，速度尚可，会做改进。

数据源来自[chinese-poetry-mysql](https://github.com/KomaBeyond/chinese-poetry-mysql) 