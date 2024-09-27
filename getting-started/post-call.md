# 通过 POST 使用接口

您可以使用命令行或任意编程语言，发送POST请求来使用图纸识别接口。



{% tabs %}
{% tab title="Shell" %}
```bash
curl -X POST http://api.holdingsky.cn/v1/tuzhi -F 'file=@tu_zhi_1.pdf'
```
{% endtab %}

{% tab title="Python" %}
```python
import requests

url = "http://api.holdingsky.cn/v1/tuzhi"
file_path = 'tu_zhi_1.jpg'
with open(file_path, 'rb') as file:
    files = {'file': file}
    response = requests.post(url, files=files)
    print(response.json())
```
{% endtab %}

{% tab title="JavaScript" %}
```html
<!DOCTYPE html>
<html lang="en">
<head></head>
<body>
    <input type="file" id="fileInput">
    <script>
        document.getElementById('fileInput').addEventListener('change', async function() {
            const file = this.files[0];
            const url = "http://api.holdingsky.cn/v1/tuzhi";
            const formData = new FormData();
            formData.append('file', file);
            const response = await fetch(url, {
                method: 'POST',
                body: formData
            });
            const jsonResponse = await response.json();
            console.log("Response received:", jsonResponse);
        });
    </script>
</body>
</html>
```
{% endtab %}

{% tab title="C#" %}
```csharp
using System;
using System.Net.Http;
using System.IO;

class Program
{
    static void Main(string[] args)
    {
        string url = "http://api.holdingsky.cn/v1/tuzhi";
        string filePath = "tu_zhi_1.jpg";
        using var client = new HttpClient();
        using var fileStream = new FileStream(filePath, FileMode.Open, FileAccess.Read);
        using var fileContent = new StreamContent(fileStream);
        using var content = new MultipartFormDataContent
        {
            { fileContent, "file", Path.GetFileName(filePath) }
        };
        var response = client.PostAsync(url, content).Result;
        response.EnsureSuccessStatusCode();
        var responseContent = response.Content.ReadAsStringAsync().Result;
        Console.WriteLine(responseContent);
    }
}
```
{% endtab %}
{% endtabs %}

在上述命令中，请将 `tu_zhi_1.pdf` 替换为您本地的图纸文件路径。文件类型支持 pdf、 jpg、 png。



[接口参数和返回值的详细信息，请访问这里](../how-to-guides/api-parameter-details.md)。
