# UpdateLoginProfile {#doc_api_977684 .reference}

修改用户的登录配置。

## 调试 {#apiExplorer .section}

前往【[API Explorer](https://api.aliyun.com/#product=Ram&api=UpdateLoginProfile)】在线调试，API Explorer 提供在线调用 API、动态生成 SDK Example 代码和快速检索接口等能力，能显著降低使用云 API 的难度，强烈推荐使用。

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|UpdateLoginProfile|系统规定参数。取值：UpdateLoginProfile

 |
|UserName|String|是|zhangqiang|指定用户名。

 |
|MFABindRequired|Boolean|否|true|指定用户在下次登录时是否必须绑定MFA。

 |
|Password|String|否|mypassword|指定密码，密码必须符合主账号的密码强度要求。

 |
|PasswordResetRequired|Boolean|否|true|指定用户在登录时是否需要修改密码。

 |

## 返回参数 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|04F0F334-1335-436C-A1D7-6C044FE73368|请求ID。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

https://ram.aliyuncs.com/?Action=UpdateLoginProfile
&UserName=zhangqiang
&Password=mypassword
&PasswordResetRequired=true
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<UpdateLoginProfile>
  <RequestId>04F0F334-1335-436C-A1D7-6C044FE73368</RequestId>
</UpdateLoginProfile>

```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"04F0F334-1335-436C-A1D7-6C044FE73368"
}
```

## 错误码 { .section}

[查看本产品错误码](https://error-center.aliyun.com/status/product/Ram)

