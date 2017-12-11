# Gyeesoft.aliyun.sdk
代码基于aliyun.sdk,迁移到.net standard 2.0,修改一些兼容性bug

兼容性bug：
1. .net core 2.0 sha1算法 using (var hashAlgorithm = new HMACSHA1(Encoding.GetBytes(key.ToCharArray())))
2.  不同平台下方法名同统一   //var internalMethodName = (_isMonoPlatform == true) ? "AddWithoutValidate" : "AddInternal"; 
    var internalMethodName = "AddWithoutValidate";
