<div align="center">
<div align="center">
<h1>API for PixelFaramitaLuminousPolymerization</h1>
<h2 align="center">对接接口文档</h2>
</div>
<div align="right"><h4>Powered by LLRemoteCall</h4></div>
</div>

> - JavaScript
>```js
>let PFLP = ll.require("PixelFaramitaLuminousPolymerization");
>```
> - C++
>```C++
>#include <RemoteCallAPI.h>
>```
> - C#
>```C#
>using RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI;
>```
> - Visual Basic .Net
>```vb
>Imports RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI
>```
> - F#
>```F#
>#r "LiteLoader.Net"
>open LiteLoader.RemoteCall
>```
> - Lua
>
> 不会写，用lua的小伙伴门看着办吧
> 滑稽

<details>
<summary><b>General<b></summary>

> <details>
> <summary><b>SetConfig  - 设置全局配置文件（要求JSON字符串）<b></summary>
>
>## General::SetConfig
>### 设置全局配置文件（要求JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| jsonStr | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 设置全局配置文件（要求JSON字符串） 返回值类型：bool */
>const General_SetConfig = ll.import("PFLP", "General::SetConfig");
>let result = General_SetConfig(jsonStr);
>```
> - C++
>```C++
>// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>auto General_SetConfig = RemoteCall::importAs<bool(std::string const& jsonStr)>("PFLP", "General::SetConfig");
>auto result = General_SetConfig(jsonStr);
>```
> - C#
>```C#
>// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>var General_SetConfig = RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig");
>var result = General_SetConfig(jsonStr);
>```
> - Visual Basic .Net
>```vb
>' 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>Dim General_SetConfig = RemoteCallAPI.ImportAs(Of Boolean,String)("PFLP", "General::SetConfig")
>Dim result = General_SetConfig(jsonStr)
>```
> - F#
>```F#
>// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>let General_SetConfig = RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig")
>jsonStr
>	|>General_SetConfig.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetConfig  - 获取全局配置文件（JSON字符串）<b></summary>
>
>## General::GetConfig
>### 获取全局配置文件（JSON字符串）
>无参数;
>返回值类型：string;
> - JavaScript
>```js
>/** 获取全局配置文件（JSON字符串） 返回值类型：string */
>const General_GetConfig = ll.import("PFLP", "General::GetConfig");
>let result = General_GetConfig();
>```
> - C++
>```C++
>// 获取全局配置文件（JSON字符串） 返回值类型：string
>auto General_GetConfig = RemoteCall::importAs<std::string()>("PFLP", "General::GetConfig");
>auto result = General_GetConfig();
>```
> - C#
>```C#
>// 获取全局配置文件（JSON字符串） 返回值类型：string
>var General_GetConfig = RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig");
>var result = General_GetConfig();
>```
> - Visual Basic .Net
>```vb
>' 获取全局配置文件（JSON字符串） 返回值类型：string
>Dim General_GetConfig = RemoteCallAPI.ImportAs(Of String)("PFLP", "General::GetConfig")
>Dim result = General_GetConfig()
>```
> - F#
>```F#
>// 获取全局配置文件（JSON字符串） 返回值类型：string
>let General_GetConfig = RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig")
>General_GetConfig()
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>Reload  - 重新加载所有功能的配置文件<b></summary>
>
>## General::Reload
>### 重新加载所有功能的配置文件
>无参数;
>无返回值;
> - JavaScript
>```js
>/** 重新加载所有功能的配置文件 */
>const General_Reload = ll.import("PFLP", "General::Reload");
>General_Reload();
>```
> - C++
>```C++
>// 重新加载所有功能的配置文件
>auto General_Reload = RemoteCall::importAs<void()>("PFLP", "General::Reload");
>General_Reload();
>```
> - C#
>```C#
>// 重新加载所有功能的配置文件
>var General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload");
>General_Reload();
>```
> - Visual Basic .Net
>```vb
>' 重新加载所有功能的配置文件
>Dim General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload")
>General_Reload()
>```
> - F#
>```F#
>// 重新加载所有功能的配置文件
>let General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload")
>General_Reload()
>```
>
> </details>
</details>
<details>
<summary><b>Command<b></summary>

> <details>
> <summary><b>SetCommandDisabled  - 设置命令禁用(可设置提示)<b></summary>
>
>## Command::SetCommandDisabled
>### 设置命令禁用(可设置提示)
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| cmd | string |
>| feedback | string |
>无返回值;
> - JavaScript
>```js
>/** 设置命令禁用(可设置提示) */
>const Command_SetCommandDisabled = ll.import("PFLP", "Command::SetCommandDisabled");
>Command_SetCommandDisabled(playerXuid,cmd,feedback);
>```
> - C++
>```C++
>// 设置命令禁用(可设置提示)
>auto Command_SetCommandDisabled = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& cmd,std::string const& feedback)>("PFLP", "Command::SetCommandDisabled");
>Command_SetCommandDisabled(playerXuid,cmd,feedback);
>```
> - C#
>```C#
>// 设置命令禁用(可设置提示)
>var Command_SetCommandDisabled = RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled");
>Command_SetCommandDisabled(playerXuid,cmd,feedback);
>```
> - Visual Basic .Net
>```vb
>' 设置命令禁用(可设置提示)
>Dim Command_SetCommandDisabled = RemoteCallAPI.Import_As(Of String,String,String)("PFLP", "Command::SetCommandDisabled")
>Command_SetCommandDisabled(playerXuid,cmd,feedback)
>```
> - F#
>```F#
>// 设置命令禁用(可设置提示)
>let Command_SetCommandDisabled = RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled")
>(playerXuid,cmd,feedback)
>	|>Command_SetCommandDisabled.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetCommandEnabled  - 设置命令启用<b></summary>
>
>## Command::SetCommandEnabled
>### 设置命令启用
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| cmd | string |
>无返回值;
> - JavaScript
>```js
>/** 设置命令启用 */
>const Command_SetCommandEnabled = ll.import("PFLP", "Command::SetCommandEnabled");
>Command_SetCommandEnabled(playerXuid,cmd);
>```
> - C++
>```C++
>// 设置命令启用
>auto Command_SetCommandEnabled = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& cmd)>("PFLP", "Command::SetCommandEnabled");
>Command_SetCommandEnabled(playerXuid,cmd);
>```
> - C#
>```C#
>// 设置命令启用
>var Command_SetCommandEnabled = RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled");
>Command_SetCommandEnabled(playerXuid,cmd);
>```
> - Visual Basic .Net
>```vb
>' 设置命令启用
>Dim Command_SetCommandEnabled = RemoteCallAPI.Import_As(Of String,String)("PFLP", "Command::SetCommandEnabled")
>Command_SetCommandEnabled(playerXuid,cmd)
>```
> - F#
>```F#
>// 设置命令启用
>let Command_SetCommandEnabled = RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled")
>(playerXuid,cmd)
>	|>Command_SetCommandEnabled.Invoke
>```
>
> </details>
</details>
<details>
<summary><b>Language<b></summary>

> <details>
> <summary><b>Translate  - 翻译<b></summary>
>
>## Language::Translate
>### 翻译
>|  形参   | 类型  |
>|  ----  | ----  |
>| fromLanguage | string |
>| toLanguage | string |
>| text | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 翻译 返回值类型：string */
>const Language_Translate = ll.import("PFLP", "Language::Translate");
>let result = Language_Translate(fromLanguage,toLanguage,text);
>```
> - C++
>```C++
>// 翻译 返回值类型：string
>auto Language_Translate = RemoteCall::importAs<std::string(std::string const& fromLanguage,std::string const& toLanguage,std::string const& text)>("PFLP", "Language::Translate");
>auto result = Language_Translate(fromLanguage,toLanguage,text);
>```
> - C#
>```C#
>// 翻译 返回值类型：string
>var Language_Translate = RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate");
>var result = Language_Translate(fromLanguage,toLanguage,text);
>```
> - Visual Basic .Net
>```vb
>' 翻译 返回值类型：string
>Dim Language_Translate = RemoteCallAPI.ImportAs(Of String,String,String,String)("PFLP", "Language::Translate")
>Dim result = Language_Translate(fromLanguage,toLanguage,text)
>```
> - F#
>```F#
>// 翻译 返回值类型：string
>let Language_Translate = RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate")
>(fromLanguage,toLanguage,text)
>	|>Language_Translate.Invoke
>	|>ignore
>```
>
> </details>
</details>
<details>
<summary><b>ChatEx<b></summary>

> <details>
> <summary><b>SetNickName  - 设置玩家昵称<b></summary>
>
>## ChatEx::SetNickName
>### 设置玩家昵称
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| nickName | string |
>无返回值;
> - JavaScript
>```js
>/** 设置玩家昵称 */
>const ChatEx_SetNickName = ll.import("PFLP", "ChatEx::SetNickName");
>ChatEx_SetNickName(playerXuid,nickName);
>```
> - C++
>```C++
>// 设置玩家昵称
>auto ChatEx_SetNickName = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& nickName)>("PFLP", "ChatEx::SetNickName");
>ChatEx_SetNickName(playerXuid,nickName);
>```
> - C#
>```C#
>// 设置玩家昵称
>var ChatEx_SetNickName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName");
>ChatEx_SetNickName(playerXuid,nickName);
>```
> - Visual Basic .Net
>```vb
>' 设置玩家昵称
>Dim ChatEx_SetNickName = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetNickName")
>ChatEx_SetNickName(playerXuid,nickName)
>```
> - F#
>```F#
>// 设置玩家昵称
>let ChatEx_SetNickName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName")
>(playerXuid,nickName)
>	|>ChatEx_SetNickName.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetFakeName  - 设置玩家聊天时的名字<b></summary>
>
>## ChatEx::SetFakeName
>### 设置玩家聊天时的名字
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| fakeName | string |
>无返回值;
> - JavaScript
>```js
>/** 设置玩家聊天时的名字 */
>const ChatEx_SetFakeName = ll.import("PFLP", "ChatEx::SetFakeName");
>ChatEx_SetFakeName(playerXuid,fakeName);
>```
> - C++
>```C++
>// 设置玩家聊天时的名字
>auto ChatEx_SetFakeName = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& fakeName)>("PFLP", "ChatEx::SetFakeName");
>ChatEx_SetFakeName(playerXuid,fakeName);
>```
> - C#
>```C#
>// 设置玩家聊天时的名字
>var ChatEx_SetFakeName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName");
>ChatEx_SetFakeName(playerXuid,fakeName);
>```
> - Visual Basic .Net
>```vb
>' 设置玩家聊天时的名字
>Dim ChatEx_SetFakeName = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetFakeName")
>ChatEx_SetFakeName(playerXuid,fakeName)
>```
> - F#
>```F#
>// 设置玩家聊天时的名字
>let ChatEx_SetFakeName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName")
>(playerXuid,fakeName)
>	|>ChatEx_SetFakeName.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetEnd  - 设置玩家聊天消息后缀<b></summary>
>
>## ChatEx::SetEnd
>### 设置玩家聊天消息后缀
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| endStr | string |
>无返回值;
> - JavaScript
>```js
>/** 设置玩家聊天消息后缀 */
>const ChatEx_SetEnd = ll.import("PFLP", "ChatEx::SetEnd");
>ChatEx_SetEnd(playerXuid,endStr);
>```
> - C++
>```C++
>// 设置玩家聊天消息后缀
>auto ChatEx_SetEnd = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& endStr)>("PFLP", "ChatEx::SetEnd");
>ChatEx_SetEnd(playerXuid,endStr);
>```
> - C#
>```C#
>// 设置玩家聊天消息后缀
>var ChatEx_SetEnd = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd");
>ChatEx_SetEnd(playerXuid,endStr);
>```
> - Visual Basic .Net
>```vb
>' 设置玩家聊天消息后缀
>Dim ChatEx_SetEnd = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetEnd")
>ChatEx_SetEnd(playerXuid,endStr)
>```
> - F#
>```F#
>// 设置玩家聊天消息后缀
>let ChatEx_SetEnd = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd")
>(playerXuid,endStr)
>	|>ChatEx_SetEnd.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetStart  - 设置玩家聊天消息前缀<b></summary>
>
>## ChatEx::SetStart
>### 设置玩家聊天消息前缀
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| startStr | string |
>无返回值;
> - JavaScript
>```js
>/** 设置玩家聊天消息前缀 */
>const ChatEx_SetStart = ll.import("PFLP", "ChatEx::SetStart");
>ChatEx_SetStart(playerXuid,startStr);
>```
> - C++
>```C++
>// 设置玩家聊天消息前缀
>auto ChatEx_SetStart = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& startStr)>("PFLP", "ChatEx::SetStart");
>ChatEx_SetStart(playerXuid,startStr);
>```
> - C#
>```C#
>// 设置玩家聊天消息前缀
>var ChatEx_SetStart = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart");
>ChatEx_SetStart(playerXuid,startStr);
>```
> - Visual Basic .Net
>```vb
>' 设置玩家聊天消息前缀
>Dim ChatEx_SetStart = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetStart")
>ChatEx_SetStart(playerXuid,startStr)
>```
> - F#
>```F#
>// 设置玩家聊天消息前缀
>let ChatEx_SetStart = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart")
>(playerXuid,startStr)
>	|>ChatEx_SetStart.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetNickName  - 获取玩家昵称<b></summary>
>
>## ChatEx::GetNickName
>### 获取玩家昵称
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取玩家昵称 返回值类型：string */
>const ChatEx_GetNickName = ll.import("PFLP", "ChatEx::GetNickName");
>let result = ChatEx_GetNickName(playerXuid);
>```
> - C++
>```C++
>// 获取玩家昵称 返回值类型：string
>auto ChatEx_GetNickName = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetNickName");
>auto result = ChatEx_GetNickName(playerXuid);
>```
> - C#
>```C#
>// 获取玩家昵称 返回值类型：string
>var ChatEx_GetNickName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName");
>var result = ChatEx_GetNickName(playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取玩家昵称 返回值类型：string
>Dim ChatEx_GetNickName = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetNickName")
>Dim result = ChatEx_GetNickName(playerXuid)
>```
> - F#
>```F#
>// 获取玩家昵称 返回值类型：string
>let ChatEx_GetNickName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName")
>playerXuid
>	|>ChatEx_GetNickName.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetFakeName  - 获取玩家聊天时的名字<b></summary>
>
>## ChatEx::GetFakeName
>### 获取玩家聊天时的名字
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取玩家聊天时的名字 返回值类型：string */
>const ChatEx_GetFakeName = ll.import("PFLP", "ChatEx::GetFakeName");
>let result = ChatEx_GetFakeName(playerXuid);
>```
> - C++
>```C++
>// 获取玩家聊天时的名字 返回值类型：string
>auto ChatEx_GetFakeName = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetFakeName");
>auto result = ChatEx_GetFakeName(playerXuid);
>```
> - C#
>```C#
>// 获取玩家聊天时的名字 返回值类型：string
>var ChatEx_GetFakeName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName");
>var result = ChatEx_GetFakeName(playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取玩家聊天时的名字 返回值类型：string
>Dim ChatEx_GetFakeName = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetFakeName")
>Dim result = ChatEx_GetFakeName(playerXuid)
>```
> - F#
>```F#
>// 获取玩家聊天时的名字 返回值类型：string
>let ChatEx_GetFakeName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName")
>playerXuid
>	|>ChatEx_GetFakeName.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetEnd  - 获取玩家聊天消息后缀<b></summary>
>
>## ChatEx::GetEnd
>### 获取玩家聊天消息后缀
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取玩家聊天消息后缀 返回值类型：string */
>const ChatEx_GetEnd = ll.import("PFLP", "ChatEx::GetEnd");
>let result = ChatEx_GetEnd(playerXuid);
>```
> - C++
>```C++
>// 获取玩家聊天消息后缀 返回值类型：string
>auto ChatEx_GetEnd = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetEnd");
>auto result = ChatEx_GetEnd(playerXuid);
>```
> - C#
>```C#
>// 获取玩家聊天消息后缀 返回值类型：string
>var ChatEx_GetEnd = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd");
>var result = ChatEx_GetEnd(playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取玩家聊天消息后缀 返回值类型：string
>Dim ChatEx_GetEnd = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetEnd")
>Dim result = ChatEx_GetEnd(playerXuid)
>```
> - F#
>```F#
>// 获取玩家聊天消息后缀 返回值类型：string
>let ChatEx_GetEnd = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd")
>playerXuid
>	|>ChatEx_GetEnd.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetStart  - 获取玩家聊天消息前缀<b></summary>
>
>## ChatEx::GetStart
>### 获取玩家聊天消息前缀
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取玩家聊天消息前缀 返回值类型：string */
>const ChatEx_GetStart = ll.import("PFLP", "ChatEx::GetStart");
>let result = ChatEx_GetStart(playerXuid);
>```
> - C++
>```C++
>// 获取玩家聊天消息前缀 返回值类型：string
>auto ChatEx_GetStart = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetStart");
>auto result = ChatEx_GetStart(playerXuid);
>```
> - C#
>```C#
>// 获取玩家聊天消息前缀 返回值类型：string
>var ChatEx_GetStart = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart");
>var result = ChatEx_GetStart(playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取玩家聊天消息前缀 返回值类型：string
>Dim ChatEx_GetStart = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetStart")
>Dim result = ChatEx_GetStart(playerXuid)
>```
> - F#
>```F#
>// 获取玩家聊天消息前缀 返回值类型：string
>let ChatEx_GetStart = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart")
>playerXuid
>	|>ChatEx_GetStart.Invoke
>	|>ignore
>```
>
> </details>
</details>
<details>
<summary><b>ParticlesGraphics<b></summary>

> <details>
> <summary><b>DrawBlock  - 给指定方块描框<b></summary>
>
>## ParticlesGraphics::DrawBlock
>### 给指定方块描框
>|  形参   | 类型  |
>|  ----  | ----  |
>| player | Player |
>| x | int |
>| y | int |
>| z | int |
>| r | float |
>| g | float |
>| b | float |
>| thickness | float |
>| time | float |
>| alpha | float |
>无返回值;
> - JavaScript
>```js
>/** 给指定方块描框 */
>const ParticlesGraphics_DrawBlock = ll.import("PFLP", "ParticlesGraphics::DrawBlock");
>ParticlesGraphics_DrawBlock(player,x,y,z,r,g,b,thickness,time,alpha);
>```
> - C++
>```C++
>// 给指定方块描框
>auto ParticlesGraphics_DrawBlock = RemoteCall::importAs<void(Player& const& player,int const& x,int const& y,int const& z,float const& r,float const& g,float const& b,float const& thickness,float const& time,float const& alpha)>("PFLP", "ParticlesGraphics::DrawBlock");
>ParticlesGraphics_DrawBlock(player,x,y,z,r,g,b,thickness,time,alpha);
>```
> - C#
>```C#
>// 给指定方块描框
>var ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As<Player,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock");
>ParticlesGraphics_DrawBlock(player,x,y,z,r,g,b,thickness,time,alpha);
>```
> - Visual Basic .Net
>```vb
>' 给指定方块描框
>Dim ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBlock")
>ParticlesGraphics_DrawBlock(player,x,y,z,r,g,b,thickness,time,alpha)
>```
> - F#
>```F#
>// 给指定方块描框
>let ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As<nativeint,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock")
>(player,x,y,z,r,g,b,thickness,time,alpha)
>	|>ParticlesGraphics_DrawBlock.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>DrawBorder  - 给指定区域描框<b></summary>
>
>## ParticlesGraphics::DrawBorder
>### 给指定区域描框
>|  形参   | 类型  |
>|  ----  | ----  |
>| player | Player |
>| x1 | int |
>| y1 | int |
>| z1 | int |
>| x2 | int |
>| y2 | int |
>| z2 | int |
>| r | float |
>| g | float |
>| b | float |
>| thickness | float |
>| time | float |
>| alpha | float |
>无返回值;
> - JavaScript
>```js
>/** 给指定区域描框 */
>const ParticlesGraphics_DrawBorder = ll.import("PFLP", "ParticlesGraphics::DrawBorder");
>ParticlesGraphics_DrawBorder(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha);
>```
> - C++
>```C++
>// 给指定区域描框
>auto ParticlesGraphics_DrawBorder = RemoteCall::importAs<void(Player& const& player,int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,float const& r,float const& g,float const& b,float const& thickness,float const& time,float const& alpha)>("PFLP", "ParticlesGraphics::DrawBorder");
>ParticlesGraphics_DrawBorder(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha);
>```
> - C#
>```C#
>// 给指定区域描框
>var ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As<Player,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder");
>ParticlesGraphics_DrawBorder(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha);
>```
> - Visual Basic .Net
>```vb
>' 给指定区域描框
>Dim ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBorder")
>ParticlesGraphics_DrawBorder(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha)
>```
> - F#
>```F#
>// 给指定区域描框
>let ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As<nativeint,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder")
>(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha)
>	|>ParticlesGraphics_DrawBorder.Invoke
>```
>
> </details>
</details>
<details>
<summary><b>Lands<b></summary>

> <details>
> <summary><b>CheckCubeHasLand  - 检查指定立方体区域(float)是否有领地<b></summary>
>
>## Lands::CheckCubeHasLand
>### 检查指定立方体区域(float)是否有领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | float |
>| y1 | float |
>| z1 | float |
>| x2 | float |
>| y2 | float |
>| z2 | float |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定立方体区域(float)是否有领地 返回值类型：bool */
>const Lands_CheckCubeHasLand = ll.import("PFLP", "Lands::CheckCubeHasLand");
>let result = Lands_CheckCubeHasLand(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 检查指定立方体区域(float)是否有领地 返回值类型：bool
>auto Lands_CheckCubeHasLand = RemoteCall::importAs<bool(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::CheckCubeHasLand");
>auto result = Lands_CheckCubeHasLand(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 检查指定立方体区域(float)是否有领地 返回值类型：bool
>var Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand");
>var result = Lands_CheckCubeHasLand(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 检查指定立方体区域(float)是否有领地 返回值类型：bool
>Dim Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::CheckCubeHasLand")
>Dim result = Lands_CheckCubeHasLand(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 检查指定立方体区域(float)是否有领地 返回值类型：bool
>let Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_CheckCubeHasLand.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckCubeHasLandInt  - 检查指定立方体区域(int)是否有领地<b></summary>
>
>## Lands::CheckCubeHasLandInt
>### 检查指定立方体区域(int)是否有领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | int |
>| y1 | int |
>| z1 | int |
>| x2 | int |
>| y2 | int |
>| z2 | int |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定立方体区域(int)是否有领地 返回值类型：bool */
>const Lands_CheckCubeHasLandInt = ll.import("PFLP", "Lands::CheckCubeHasLandInt");
>let result = Lands_CheckCubeHasLandInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 检查指定立方体区域(int)是否有领地 返回值类型：bool
>auto Lands_CheckCubeHasLandInt = RemoteCall::importAs<bool(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::CheckCubeHasLandInt");
>auto result = Lands_CheckCubeHasLandInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 检查指定立方体区域(int)是否有领地 返回值类型：bool
>var Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt");
>var result = Lands_CheckCubeHasLandInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 检查指定立方体区域(int)是否有领地 返回值类型：bool
>Dim Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckCubeHasLandInt")
>Dim result = Lands_CheckCubeHasLandInt(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 检查指定立方体区域(int)是否有领地 返回值类型：bool
>let Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_CheckCubeHasLandInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPosHasLand  - 检查指定坐标(float)是否有领地<b></summary>
>
>## Lands::CheckPosHasLand
>### 检查指定坐标(float)是否有领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(float)是否有领地 返回值类型：bool */
>const Lands_CheckPosHasLand = ll.import("PFLP", "Lands::CheckPosHasLand");
>let result = Lands_CheckPosHasLand(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 检查指定坐标(float)是否有领地 返回值类型：bool
>auto Lands_CheckPosHasLand = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::CheckPosHasLand");
>auto result = Lands_CheckPosHasLand(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 检查指定坐标(float)是否有领地 返回值类型：bool
>var Lands_CheckPosHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand");
>var result = Lands_CheckPosHasLand(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(float)是否有领地 返回值类型：bool
>Dim Lands_CheckPosHasLand = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::CheckPosHasLand")
>Dim result = Lands_CheckPosHasLand(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 检查指定坐标(float)是否有领地 返回值类型：bool
>let Lands_CheckPosHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand")
>(x,y,z,dimensionId)
>	|>Lands_CheckPosHasLand.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPosHasLandInt  - 检查指定坐标(int)是否有领地<b></summary>
>
>## Lands::CheckPosHasLandInt
>### 检查指定坐标(int)是否有领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(int)是否有领地 返回值类型：bool */
>const Lands_CheckPosHasLandInt = ll.import("PFLP", "Lands::CheckPosHasLandInt");
>let result = Lands_CheckPosHasLandInt(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 检查指定坐标(int)是否有领地 返回值类型：bool
>auto Lands_CheckPosHasLandInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::CheckPosHasLandInt");
>auto result = Lands_CheckPosHasLandInt(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 检查指定坐标(int)是否有领地 返回值类型：bool
>var Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt");
>var result = Lands_CheckPosHasLandInt(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(int)是否有领地 返回值类型：bool
>Dim Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckPosHasLandInt")
>Dim result = Lands_CheckPosHasLandInt(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 检查指定坐标(int)是否有领地 返回值类型：bool
>let Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt")
>(x,y,z,dimensionId)
>	|>Lands_CheckPosHasLandInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandByCube  - 获取立方体区域(float)领地信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandByCube
>### 获取立方体区域(float)领地信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | float |
>| y1 | float |
>| z1 | float |
>| x2 | float |
>| y2 | float |
>| z2 | float |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByCube = ll.import("PFLP", "Lands::GetLandByCube");
>let result = Lands_GetLandByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandByCube = RemoteCall::importAs<std::string(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandByCube");
>auto result = Lands_GetLandByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube");
>var result = Lands_GetLandByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByCube = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByCube")
>Dim result = Lands_GetLandByCube(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_GetLandByCube.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandByCubeInt  - 获取立方体区域(int)领地信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandByCubeInt
>### 获取立方体区域(int)领地信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | int |
>| y1 | int |
>| z1 | int |
>| x2 | int |
>| y2 | int |
>| z2 | int |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByCubeInt = ll.import("PFLP", "Lands::GetLandByCubeInt");
>let result = Lands_GetLandByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandByCubeInt = RemoteCall::importAs<std::string(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandByCubeInt");
>auto result = Lands_GetLandByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt");
>var result = Lands_GetLandByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByCubeInt")
>Dim result = Lands_GetLandByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_GetLandByCubeInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandByPos  - 获取指定坐标(float)领地信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandByPos
>### 获取指定坐标(float)领地信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByPos = ll.import("PFLP", "Lands::GetLandByPos");
>let result = Lands_GetLandByPos(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::GetLandByPos");
>auto result = Lands_GetLandByPos(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos");
>var result = Lands_GetLandByPos(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByPos")
>Dim result = Lands_GetLandByPos(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos")
>(x,y,z,dimensionId)
>	|>Lands_GetLandByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandByPosInt  - 获取指定坐标(int)领地信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandByPosInt
>### 获取指定坐标(int)领地信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByPosInt = ll.import("PFLP", "Lands::GetLandByPosInt");
>let result = Lands_GetLandByPosInt(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::GetLandByPosInt");
>auto result = Lands_GetLandByPosInt(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt");
>var result = Lands_GetLandByPosInt(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByPosInt")
>Dim result = Lands_GetLandByPosInt(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt")
>(x,y,z,dimensionId)
>	|>Lands_GetLandByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandInfoByCube  - 获取立方体区域(float)领地数据源详细信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandInfoByCube
>### 获取立方体区域(float)领地数据源详细信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | float |
>| y1 | float |
>| z1 | float |
>| x2 | float |
>| y2 | float |
>| z2 | float |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByCube = ll.import("PFLP", "Lands::GetLandInfoByCube");
>let result = Lands_GetLandInfoByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandInfoByCube = RemoteCall::importAs<std::string(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByCube");
>auto result = Lands_GetLandInfoByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube");
>var result = Lands_GetLandInfoByCube(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByCube")
>Dim result = Lands_GetLandInfoByCube(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_GetLandInfoByCube.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandInfoByCubeInt  - 获取立方体区域(int)领地数据源详细信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandInfoByCubeInt
>### 获取立方体区域(int)领地数据源详细信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | int |
>| y1 | int |
>| z1 | int |
>| x2 | int |
>| y2 | int |
>| z2 | int |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByCubeInt = ll.import("PFLP", "Lands::GetLandInfoByCubeInt");
>let result = Lands_GetLandInfoByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C++
>```C++
>// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandInfoByCubeInt = RemoteCall::importAs<std::string(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByCubeInt");
>auto result = Lands_GetLandInfoByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - C#
>```C#
>// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt");
>var result = Lands_GetLandInfoByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByCubeInt")
>Dim result = Lands_GetLandInfoByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId)
>```
> - F#
>```F#
>// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt")
>(x1,y1,z1,x2,y2,z2,dimensionId)
>	|>Lands_GetLandInfoByCubeInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandInfoByPos  - 获取指定坐标(float)领地数据源详细信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandInfoByPos
>### 获取指定坐标(float)领地数据源详细信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByPos = ll.import("PFLP", "Lands::GetLandInfoByPos");
>let result = Lands_GetLandInfoByPos(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandInfoByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByPos");
>auto result = Lands_GetLandInfoByPos(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos");
>var result = Lands_GetLandInfoByPos(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByPos")
>Dim result = Lands_GetLandInfoByPos(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos")
>(x,y,z,dimensionId)
>	|>Lands_GetLandInfoByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandInfoByPosInt  - 获取指定坐标(int)领地数据源详细信息（返回JSON字符串）<b></summary>
>
>## Lands::GetLandInfoByPosInt
>### 获取指定坐标(int)领地数据源详细信息（返回JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByPosInt = ll.import("PFLP", "Lands::GetLandInfoByPosInt");
>let result = Lands_GetLandInfoByPosInt(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>auto Lands_GetLandInfoByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByPosInt");
>auto result = Lands_GetLandInfoByPosInt(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt");
>var result = Lands_GetLandInfoByPosInt(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByPosInt")
>Dim result = Lands_GetLandInfoByPosInt(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt")
>(x,y,z,dimensionId)
>	|>Lands_GetLandInfoByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetLandInfoByPos  - 设置指定坐标(float)领地数据源详细信息（传入JSON字符串）<b></summary>
>
>## Lands::SetLandInfoByPos
>### 设置指定坐标(float)领地数据源详细信息（传入JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>| landinfo | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool */
>const Lands_SetLandInfoByPos = ll.import("PFLP", "Lands::SetLandInfoByPos");
>let result = Lands_SetLandInfoByPos(x,y,z,dimensionId,landinfo);
>```
> - C++
>```C++
>// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>auto Lands_SetLandInfoByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& landinfo)>("PFLP", "Lands::SetLandInfoByPos");
>auto result = Lands_SetLandInfoByPos(x,y,z,dimensionId,landinfo);
>```
> - C#
>```C#
>// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>var Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos");
>var result = Lands_SetLandInfoByPos(x,y,z,dimensionId,landinfo);
>```
> - Visual Basic .Net
>```vb
>' 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>Dim Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::SetLandInfoByPos")
>Dim result = Lands_SetLandInfoByPos(x,y,z,dimensionId,landinfo)
>```
> - F#
>```F#
>// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>let Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos")
>(x,y,z,dimensionId,landinfo)
>	|>Lands_SetLandInfoByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>SetLandInfoByPosInt  - 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串）<b></summary>
>
>## Lands::SetLandInfoByPosInt
>### 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| landinfo | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool */
>const Lands_SetLandInfoByPosInt = ll.import("PFLP", "Lands::SetLandInfoByPosInt");
>let result = Lands_SetLandInfoByPosInt(x,y,z,dimensionId,landinfo);
>```
> - C++
>```C++
>// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>auto Lands_SetLandInfoByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& landinfo)>("PFLP", "Lands::SetLandInfoByPosInt");
>auto result = Lands_SetLandInfoByPosInt(x,y,z,dimensionId,landinfo);
>```
> - C#
>```C#
>// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>var Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt");
>var result = Lands_SetLandInfoByPosInt(x,y,z,dimensionId,landinfo);
>```
> - Visual Basic .Net
>```vb
>' 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>Dim Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::SetLandInfoByPosInt")
>Dim result = Lands_SetLandInfoByPosInt(x,y,z,dimensionId,landinfo)
>```
> - F#
>```F#
>// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>let Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt")
>(x,y,z,dimensionId,landinfo)
>	|>Lands_SetLandInfoByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CreateLand2D  - 新建领地<b></summary>
>
>## Lands::CreateLand2D
>### 新建领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | int |
>| z1 | int |
>| x2 | int |
>| z2 | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 新建领地 返回值类型：bool */
>const Lands_CreateLand2D = ll.import("PFLP", "Lands::CreateLand2D");
>let result = Lands_CreateLand2D(x1,z1,x2,z2,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 新建领地 返回值类型：bool
>auto Lands_CreateLand2D = RemoteCall::importAs<bool(int const& x1,int const& z1,int const& x2,int const& z2,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CreateLand2D");
>auto result = Lands_CreateLand2D(x1,z1,x2,z2,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 新建领地 返回值类型：bool
>var Lands_CreateLand2D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D");
>var result = Lands_CreateLand2D(x1,z1,x2,z2,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 新建领地 返回值类型：bool
>Dim Lands_CreateLand2D = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand2D")
>Dim result = Lands_CreateLand2D(x1,z1,x2,z2,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 新建领地 返回值类型：bool
>let Lands_CreateLand2D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D")
>(x1,z1,x2,z2,dimensionId,playerXuid)
>	|>Lands_CreateLand2D.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CreateLand3D  - 新建领地<b></summary>
>
>## Lands::CreateLand3D
>### 新建领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x1 | int |
>| y1 | int |
>| z1 | int |
>| x2 | int |
>| y2 | int |
>| z2 | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 新建领地 返回值类型：bool */
>const Lands_CreateLand3D = ll.import("PFLP", "Lands::CreateLand3D");
>let result = Lands_CreateLand3D(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 新建领地 返回值类型：bool
>auto Lands_CreateLand3D = RemoteCall::importAs<bool(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CreateLand3D");
>auto result = Lands_CreateLand3D(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 新建领地 返回值类型：bool
>var Lands_CreateLand3D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D");
>var result = Lands_CreateLand3D(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 新建领地 返回值类型：bool
>Dim Lands_CreateLand3D = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand3D")
>Dim result = Lands_CreateLand3D(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 新建领地 返回值类型：bool
>let Lands_CreateLand3D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D")
>(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid)
>	|>Lands_CreateLand3D.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>DeleteLandByPos  - 删除指定坐标(float)的领地<b></summary>
>
>## Lands::DeleteLandByPos
>### 删除指定坐标(float)的领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 删除指定坐标(float)的领地 返回值类型：bool */
>const Lands_DeleteLandByPos = ll.import("PFLP", "Lands::DeleteLandByPos");
>let result = Lands_DeleteLandByPos(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 删除指定坐标(float)的领地 返回值类型：bool
>auto Lands_DeleteLandByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::DeleteLandByPos");
>auto result = Lands_DeleteLandByPos(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 删除指定坐标(float)的领地 返回值类型：bool
>var Lands_DeleteLandByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos");
>var result = Lands_DeleteLandByPos(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 删除指定坐标(float)的领地 返回值类型：bool
>Dim Lands_DeleteLandByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::DeleteLandByPos")
>Dim result = Lands_DeleteLandByPos(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 删除指定坐标(float)的领地 返回值类型：bool
>let Lands_DeleteLandByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos")
>(x,y,z,dimensionId)
>	|>Lands_DeleteLandByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>DeleteLandByPosInt  - 删除指定坐标(int)的领地<b></summary>
>
>## Lands::DeleteLandByPosInt
>### 删除指定坐标(int)的领地
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>返回值类型：bool;
> - JavaScript
>```js
>/** 删除指定坐标(int)的领地 返回值类型：bool */
>const Lands_DeleteLandByPosInt = ll.import("PFLP", "Lands::DeleteLandByPosInt");
>let result = Lands_DeleteLandByPosInt(x,y,z,dimensionId);
>```
> - C++
>```C++
>// 删除指定坐标(int)的领地 返回值类型：bool
>auto Lands_DeleteLandByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::DeleteLandByPosInt");
>auto result = Lands_DeleteLandByPosInt(x,y,z,dimensionId);
>```
> - C#
>```C#
>// 删除指定坐标(int)的领地 返回值类型：bool
>var Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt");
>var result = Lands_DeleteLandByPosInt(x,y,z,dimensionId);
>```
> - Visual Basic .Net
>```vb
>' 删除指定坐标(int)的领地 返回值类型：bool
>Dim Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::DeleteLandByPosInt")
>Dim result = Lands_DeleteLandByPosInt(x,y,z,dimensionId)
>```
> - F#
>```F#
>// 删除指定坐标(int)的领地 返回值类型：bool
>let Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt")
>(x,y,z,dimensionId)
>	|>Lands_DeleteLandByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandPermissionByPos  - 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）<b></summary>
>
>## Lands::GetLandPermissionByPos
>### 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string */
>const Lands_GetLandPermissionByPos = ll.import("PFLP", "Lands::GetLandPermissionByPos");
>let result = Lands_GetLandPermissionByPos(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>auto Lands_GetLandPermissionByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::GetLandPermissionByPos");
>auto result = Lands_GetLandPermissionByPos(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>var Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos");
>var result = Lands_GetLandPermissionByPos(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>Dim Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer,String)("PFLP", "Lands::GetLandPermissionByPos")
>Dim result = Lands_GetLandPermissionByPos(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>let Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_GetLandPermissionByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>GetLandPermissionByPosInt  - 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）<b></summary>
>
>## Lands::GetLandPermissionByPosInt
>### 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：string;
> - JavaScript
>```js
>/** 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string */
>const Lands_GetLandPermissionByPosInt = ll.import("PFLP", "Lands::GetLandPermissionByPosInt");
>let result = Lands_GetLandPermissionByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>auto Lands_GetLandPermissionByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::GetLandPermissionByPosInt");
>auto result = Lands_GetLandPermissionByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>var Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt");
>var result = Lands_GetLandPermissionByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>Dim Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::GetLandPermissionByPosInt")
>Dim result = Lands_GetLandPermissionByPosInt(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>let Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_GetLandPermissionByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckLandPermissionByPos  - 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）<b></summary>
>
>## Lands::CheckLandPermissionByPos
>### 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| permissionId | string |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool */
>const Lands_CheckLandPermissionByPos = ll.import("PFLP", "Lands::CheckLandPermissionByPos");
>let result = Lands_CheckLandPermissionByPos(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>auto Lands_CheckLandPermissionByPos = RemoteCall::importAs<bool(std::string const& permissionId,float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckLandPermissionByPos");
>auto result = Lands_CheckLandPermissionByPos(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>var Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos");
>var result = Lands_CheckLandPermissionByPos(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>Dim Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs(Of Boolean,String,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckLandPermissionByPos")
>Dim result = Lands_CheckLandPermissionByPos(permissionId,x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>let Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos")
>(permissionId,x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckLandPermissionByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckLandPermissionByPosInt  - 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）<b></summary>
>
>## Lands::CheckLandPermissionByPosInt
>### 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串）
>|  形参   | 类型  |
>|  ----  | ----  |
>| permissionId | string |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool */
>const Lands_CheckLandPermissionByPosInt = ll.import("PFLP", "Lands::CheckLandPermissionByPosInt");
>let result = Lands_CheckLandPermissionByPosInt(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>auto Lands_CheckLandPermissionByPosInt = RemoteCall::importAs<bool(std::string const& permissionId,int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckLandPermissionByPosInt");
>auto result = Lands_CheckLandPermissionByPosInt(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>var Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt");
>var result = Lands_CheckLandPermissionByPosInt(permissionId,x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>Dim Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs(Of Boolean,String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckLandPermissionByPosInt")
>Dim result = Lands_CheckLandPermissionByPosInt(permissionId,x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>let Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt")
>(permissionId,x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckLandPermissionByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPlayerIsLandOwnerByPos  - 检查玩家是否是指定坐标(float)领地的主人<b></summary>
>
>## Lands::CheckPlayerIsLandOwnerByPos
>### 检查玩家是否是指定坐标(float)领地的主人
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool */
>const Lands_CheckPlayerIsLandOwnerByPos = ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
>let result = Lands_CheckPlayerIsLandOwnerByPos(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>auto Lands_CheckPlayerIsLandOwnerByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
>auto result = Lands_CheckPlayerIsLandOwnerByPos(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>var Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
>var result = Lands_CheckPlayerIsLandOwnerByPos(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>Dim Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPos")
>Dim result = Lands_CheckPlayerIsLandOwnerByPos(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>let Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckPlayerIsLandOwnerByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPlayerIsLandOwnerByPosInt  - 检查玩家是否是指定坐标(int)领地的主人<b></summary>
>
>## Lands::CheckPlayerIsLandOwnerByPosInt
>### 检查玩家是否是指定坐标(int)领地的主人
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool */
>const Lands_CheckPlayerIsLandOwnerByPosInt = ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
>let result = Lands_CheckPlayerIsLandOwnerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>auto Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
>auto result = Lands_CheckPlayerIsLandOwnerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>var Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
>var result = Lands_CheckPlayerIsLandOwnerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>Dim Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt")
>Dim result = Lands_CheckPlayerIsLandOwnerByPosInt(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>let Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckPlayerIsLandOwnerByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckIsLandSharedToPlayerByPos  - 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos）<b></summary>
>
>## Lands::CheckIsLandSharedToPlayerByPos
>### 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | float |
>| y | float |
>| z | float |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool */
>const Lands_CheckIsLandSharedToPlayerByPos = ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
>let result = Lands_CheckIsLandSharedToPlayerByPos(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>auto Lands_CheckIsLandSharedToPlayerByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
>auto result = Lands_CheckIsLandSharedToPlayerByPos(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>var Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
>var result = Lands_CheckIsLandSharedToPlayerByPos(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>Dim Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPos")
>Dim result = Lands_CheckIsLandSharedToPlayerByPos(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>let Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckIsLandSharedToPlayerByPos.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckIsLandSharedToPlayerByPosInt  - 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos）<b></summary>
>
>## Lands::CheckIsLandSharedToPlayerByPosInt
>### 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos）
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool */
>const Lands_CheckIsLandSharedToPlayerByPosInt = ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
>let result = Lands_CheckIsLandSharedToPlayerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>auto Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
>auto result = Lands_CheckIsLandSharedToPlayerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>var Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
>var result = Lands_CheckIsLandSharedToPlayerByPosInt(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>Dim Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt")
>Dim result = Lands_CheckIsLandSharedToPlayerByPosInt(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>let Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckIsLandSharedToPlayerByPosInt.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPlayerHasCreateChestPermission  - 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件)<b></summary>
>
>## Lands::CheckPlayerHasCreateChestPermission
>### 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件)
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool */
>const Lands_CheckPlayerHasCreateChestPermission = ll.import("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
>let result = Lands_CheckPlayerHasCreateChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>auto Lands_CheckPlayerHasCreateChestPermission = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
>auto result = Lands_CheckPlayerHasCreateChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>var Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
>var result = Lands_CheckPlayerHasCreateChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>Dim Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasCreateChestPermission")
>Dim result = Lands_CheckPlayerHasCreateChestPermission(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>let Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckPlayerHasCreateChestPermission.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>CheckPlayerHasOpenChestPermission  - 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件)<b></summary>
>
>## Lands::CheckPlayerHasOpenChestPermission
>### 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件)
>|  形参   | 类型  |
>|  ----  | ----  |
>| x | int |
>| y | int |
>| z | int |
>| dimensionId | int |
>| playerXuid | string |
>返回值类型：bool;
> - JavaScript
>```js
>/** 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool */
>const Lands_CheckPlayerHasOpenChestPermission = ll.import("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
>let result = Lands_CheckPlayerHasOpenChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - C++
>```C++
>// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>auto Lands_CheckPlayerHasOpenChestPermission = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
>auto result = Lands_CheckPlayerHasOpenChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - C#
>```C#
>// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>var Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
>var result = Lands_CheckPlayerHasOpenChestPermission(x,y,z,dimensionId,playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>Dim Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasOpenChestPermission")
>Dim result = Lands_CheckPlayerHasOpenChestPermission(x,y,z,dimensionId,playerXuid)
>```
> - F#
>```F#
>// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>let Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission")
>(x,y,z,dimensionId,playerXuid)
>	|>Lands_CheckPlayerHasOpenChestPermission.Invoke
>	|>ignore
>```
>
> </details>
</details>
<details>
<summary><b>Money<b></summary>

> <details>
> <summary><b>Get  - 获取玩家(指定玩家名)金钱<b></summary>
>
>## Money::Get
>### 获取玩家(指定玩家名)金钱
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>返回值类型：long;
> - JavaScript
>```js
>/** 获取玩家(指定玩家名)金钱 返回值类型：long */
>const Money_Get = ll.import("PFLP", "Money::Get");
>let result = Money_Get(playerXuid);
>```
> - C++
>```C++
>// 获取玩家(指定玩家名)金钱 返回值类型：long
>auto Money_Get = RemoteCall::importAs<long long(std::string const& playerXuid)>("PFLP", "Money::Get");
>auto result = Money_Get(playerXuid);
>```
> - C#
>```C#
>// 获取玩家(指定玩家名)金钱 返回值类型：long
>var Money_Get = RemoteCallAPI.ImportAs<long,string>("PFLP", "Money::Get");
>var result = Money_Get(playerXuid);
>```
> - Visual Basic .Net
>```vb
>' 获取玩家(指定玩家名)金钱 返回值类型：long
>Dim Money_Get = RemoteCallAPI.ImportAs(Of Long,String)("PFLP", "Money::Get")
>Dim result = Money_Get(playerXuid)
>```
> - F#
>```F#
>// 获取玩家(指定玩家名)金钱 返回值类型：long
>let Money_Get = RemoteCallAPI.ImportAs<int64,string>("PFLP", "Money::Get")
>playerXuid
>	|>Money_Get.Invoke
>	|>ignore
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>Add  - 给玩家(指定玩家名)加钱<b></summary>
>
>## Money::Add
>### 给玩家(指定玩家名)加钱
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| count | long |
>| info | string |
>无返回值;
> - JavaScript
>```js
>/** 给玩家(指定玩家名)加钱 */
>const Money_Add = ll.import("PFLP", "Money::Add");
>Money_Add(playerXuid,count,info);
>```
> - C++
>```C++
>// 给玩家(指定玩家名)加钱
>auto Money_Add = RemoteCall::importAs<void(std::string const& playerXuid,long long const& count,std::string const& info)>("PFLP", "Money::Add");
>Money_Add(playerXuid,count,info);
>```
> - C#
>```C#
>// 给玩家(指定玩家名)加钱
>var Money_Add = RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Add");
>Money_Add(playerXuid,count,info);
>```
> - Visual Basic .Net
>```vb
>' 给玩家(指定玩家名)加钱
>Dim Money_Add = RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Add")
>Money_Add(playerXuid,count,info)
>```
> - F#
>```F#
>// 给玩家(指定玩家名)加钱
>let Money_Add = RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Add")
>(playerXuid,count,info)
>	|>Money_Add.Invoke
>```
>
> </details>
>
>---
>
> <details>
> <summary><b>Remove  - 给玩家(指定玩家名)减钱<b></summary>
>
>## Money::Remove
>### 给玩家(指定玩家名)减钱
>|  形参   | 类型  |
>|  ----  | ----  |
>| playerXuid | string |
>| count | long |
>| info | string |
>无返回值;
> - JavaScript
>```js
>/** 给玩家(指定玩家名)减钱 */
>const Money_Remove = ll.import("PFLP", "Money::Remove");
>Money_Remove(playerXuid,count,info);
>```
> - C++
>```C++
>// 给玩家(指定玩家名)减钱
>auto Money_Remove = RemoteCall::importAs<void(std::string const& playerXuid,long long const& count,std::string const& info)>("PFLP", "Money::Remove");
>Money_Remove(playerXuid,count,info);
>```
> - C#
>```C#
>// 给玩家(指定玩家名)减钱
>var Money_Remove = RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Remove");
>Money_Remove(playerXuid,count,info);
>```
> - Visual Basic .Net
>```vb
>' 给玩家(指定玩家名)减钱
>Dim Money_Remove = RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Remove")
>Money_Remove(playerXuid,count,info)
>```
> - F#
>```F#
>// 给玩家(指定玩家名)减钱
>let Money_Remove = RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Remove")
>(playerXuid,count,info)
>	|>Money_Remove.Invoke
>```
>
> </details>
</details>
<details><summary><b>All Api in JavaScript / JS接口<b></summary>


>---
><details><summary>JavaScript imports / 逐个导入</summary>
>
>``` JavaScript
>/** 设置全局配置文件（要求JSON字符串） 返回值类型：bool */
>const General_SetConfig = ll.import("PFLP", "General::SetConfig");
>/** 获取全局配置文件（JSON字符串） 返回值类型：string */
>const General_GetConfig = ll.import("PFLP", "General::GetConfig");
>/** 重新加载所有功能的配置文件 */
>const General_Reload = ll.import("PFLP", "General::Reload");
>/** 设置命令禁用(可设置提示) */
>const Command_SetCommandDisabled = ll.import("PFLP", "Command::SetCommandDisabled");
>/** 设置命令启用 */
>const Command_SetCommandEnabled = ll.import("PFLP", "Command::SetCommandEnabled");
>/** 翻译 返回值类型：string */
>const Language_Translate = ll.import("PFLP", "Language::Translate");
>/** 设置玩家昵称 */
>const ChatEx_SetNickName = ll.import("PFLP", "ChatEx::SetNickName");
>/** 设置玩家聊天时的名字 */
>const ChatEx_SetFakeName = ll.import("PFLP", "ChatEx::SetFakeName");
>/** 设置玩家聊天消息后缀 */
>const ChatEx_SetEnd = ll.import("PFLP", "ChatEx::SetEnd");
>/** 设置玩家聊天消息前缀 */
>const ChatEx_SetStart = ll.import("PFLP", "ChatEx::SetStart");
>/** 获取玩家昵称 返回值类型：string */
>const ChatEx_GetNickName = ll.import("PFLP", "ChatEx::GetNickName");
>/** 获取玩家聊天时的名字 返回值类型：string */
>const ChatEx_GetFakeName = ll.import("PFLP", "ChatEx::GetFakeName");
>/** 获取玩家聊天消息后缀 返回值类型：string */
>const ChatEx_GetEnd = ll.import("PFLP", "ChatEx::GetEnd");
>/** 获取玩家聊天消息前缀 返回值类型：string */
>const ChatEx_GetStart = ll.import("PFLP", "ChatEx::GetStart");
>/** 给指定方块描框 */
>const ParticlesGraphics_DrawBlock = ll.import("PFLP", "ParticlesGraphics::DrawBlock");
>/** 给指定区域描框 */
>const ParticlesGraphics_DrawBorder = ll.import("PFLP", "ParticlesGraphics::DrawBorder");
>/** 检查指定立方体区域(float)是否有领地 返回值类型：bool */
>const Lands_CheckCubeHasLand = ll.import("PFLP", "Lands::CheckCubeHasLand");
>/** 检查指定立方体区域(int)是否有领地 返回值类型：bool */
>const Lands_CheckCubeHasLandInt = ll.import("PFLP", "Lands::CheckCubeHasLandInt");
>/** 检查指定坐标(float)是否有领地 返回值类型：bool */
>const Lands_CheckPosHasLand = ll.import("PFLP", "Lands::CheckPosHasLand");
>/** 检查指定坐标(int)是否有领地 返回值类型：bool */
>const Lands_CheckPosHasLandInt = ll.import("PFLP", "Lands::CheckPosHasLandInt");
>/** 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByCube = ll.import("PFLP", "Lands::GetLandByCube");
>/** 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByCubeInt = ll.import("PFLP", "Lands::GetLandByCubeInt");
>/** 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByPos = ll.import("PFLP", "Lands::GetLandByPos");
>/** 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandByPosInt = ll.import("PFLP", "Lands::GetLandByPosInt");
>/** 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByCube = ll.import("PFLP", "Lands::GetLandInfoByCube");
>/** 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByCubeInt = ll.import("PFLP", "Lands::GetLandInfoByCubeInt");
>/** 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByPos = ll.import("PFLP", "Lands::GetLandInfoByPos");
>/** 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string */
>const Lands_GetLandInfoByPosInt = ll.import("PFLP", "Lands::GetLandInfoByPosInt");
>/** 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool */
>const Lands_SetLandInfoByPos = ll.import("PFLP", "Lands::SetLandInfoByPos");
>/** 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool */
>const Lands_SetLandInfoByPosInt = ll.import("PFLP", "Lands::SetLandInfoByPosInt");
>/** 新建领地 返回值类型：bool */
>const Lands_CreateLand2D = ll.import("PFLP", "Lands::CreateLand2D");
>/** 新建领地 返回值类型：bool */
>const Lands_CreateLand3D = ll.import("PFLP", "Lands::CreateLand3D");
>/** 删除指定坐标(float)的领地 返回值类型：bool */
>const Lands_DeleteLandByPos = ll.import("PFLP", "Lands::DeleteLandByPos");
>/** 删除指定坐标(int)的领地 返回值类型：bool */
>const Lands_DeleteLandByPosInt = ll.import("PFLP", "Lands::DeleteLandByPosInt");
>/** 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string */
>const Lands_GetLandPermissionByPos = ll.import("PFLP", "Lands::GetLandPermissionByPos");
>/** 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string */
>const Lands_GetLandPermissionByPosInt = ll.import("PFLP", "Lands::GetLandPermissionByPosInt");
>/** 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool */
>const Lands_CheckLandPermissionByPos = ll.import("PFLP", "Lands::CheckLandPermissionByPos");
>/** 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool */
>const Lands_CheckLandPermissionByPosInt = ll.import("PFLP", "Lands::CheckLandPermissionByPosInt");
>/** 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool */
>const Lands_CheckPlayerIsLandOwnerByPos = ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
>/** 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool */
>const Lands_CheckPlayerIsLandOwnerByPosInt = ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
>/** 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool */
>const Lands_CheckIsLandSharedToPlayerByPos = ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
>/** 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool */
>const Lands_CheckIsLandSharedToPlayerByPosInt = ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
>/** 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool */
>const Lands_CheckPlayerHasCreateChestPermission = ll.import("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
>/** 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool */
>const Lands_CheckPlayerHasOpenChestPermission = ll.import("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
>/** 获取玩家(指定玩家名)金钱 返回值类型：long */
>const Money_Get = ll.import("PFLP", "Money::Get");
>/** 给玩家(指定玩家名)加钱 */
>const Money_Add = ll.import("PFLP", "Money::Add");
>/** 给玩家(指定玩家名)减钱 */
>const Money_Remove = ll.import("PFLP", "Money::Remove");
>
>```
></details>
><details><summary>JavaScript object / JS对象 （推荐）</summary>
>
>``` JavaScript
>const PFLP = {
>	General : {
>		/** 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>		 * @param {string} jsonStr
>		 * @returns {boolean}
>		 */
>		SetConfig(jsonStr) { return (this.General_SetConfig??=ll.import("PFLP", "General::SetConfig"))(jsonStr)},
>		/** 获取全局配置文件（JSON字符串） 返回值类型：string
>		 * @returns {string}
>		 */
>		GetConfig() { return (this.General_GetConfig??=ll.import("PFLP", "General::GetConfig"))()},
>		/** 重新加载所有功能的配置文件
>		 */
>		Reload() { (this.General_Reload??=ll.import("PFLP", "General::Reload"))()},
>	},
>	Command : {
>		/** 设置命令禁用(可设置提示)
>		 * @param {string} playerXuid
>		 * @param {string} cmd
>		 * @param {string} feedback
>		 */
>		SetCommandDisabled(playerXuid,cmd,feedback) { (this.Command_SetCommandDisabled??=ll.import("PFLP", "Command::SetCommandDisabled"))(playerXuid,cmd,feedback)},
>		/** 设置命令启用
>		 * @param {string} playerXuid
>		 * @param {string} cmd
>		 */
>		SetCommandEnabled(playerXuid,cmd) { (this.Command_SetCommandEnabled??=ll.import("PFLP", "Command::SetCommandEnabled"))(playerXuid,cmd)},
>	},
>	Language : {
>		/** 翻译 返回值类型：string
>		 * @param {string} fromLanguage
>		 * @param {string} toLanguage
>		 * @param {string} text
>		 * @returns {string}
>		 */
>		Translate(fromLanguage,toLanguage,text) { return (this.Language_Translate??=ll.import("PFLP", "Language::Translate"))(fromLanguage,toLanguage,text)},
>	},
>	ChatEx : {
>		/** 设置玩家昵称
>		 * @param {string} playerXuid
>		 * @param {string} nickName
>		 */
>		SetNickName(playerXuid,nickName) { (this.ChatEx_SetNickName??=ll.import("PFLP", "ChatEx::SetNickName"))(playerXuid,nickName)},
>		/** 设置玩家聊天时的名字
>		 * @param {string} playerXuid
>		 * @param {string} fakeName
>		 */
>		SetFakeName(playerXuid,fakeName) { (this.ChatEx_SetFakeName??=ll.import("PFLP", "ChatEx::SetFakeName"))(playerXuid,fakeName)},
>		/** 设置玩家聊天消息后缀
>		 * @param {string} playerXuid
>		 * @param {string} endStr
>		 */
>		SetEnd(playerXuid,endStr) { (this.ChatEx_SetEnd??=ll.import("PFLP", "ChatEx::SetEnd"))(playerXuid,endStr)},
>		/** 设置玩家聊天消息前缀
>		 * @param {string} playerXuid
>		 * @param {string} startStr
>		 */
>		SetStart(playerXuid,startStr) { (this.ChatEx_SetStart??=ll.import("PFLP", "ChatEx::SetStart"))(playerXuid,startStr)},
>		/** 获取玩家昵称 返回值类型：string
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetNickName(playerXuid) { return (this.ChatEx_GetNickName??=ll.import("PFLP", "ChatEx::GetNickName"))(playerXuid)},
>		/** 获取玩家聊天时的名字 返回值类型：string
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetFakeName(playerXuid) { return (this.ChatEx_GetFakeName??=ll.import("PFLP", "ChatEx::GetFakeName"))(playerXuid)},
>		/** 获取玩家聊天消息后缀 返回值类型：string
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetEnd(playerXuid) { return (this.ChatEx_GetEnd??=ll.import("PFLP", "ChatEx::GetEnd"))(playerXuid)},
>		/** 获取玩家聊天消息前缀 返回值类型：string
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetStart(playerXuid) { return (this.ChatEx_GetStart??=ll.import("PFLP", "ChatEx::GetStart"))(playerXuid)},
>	},
>	ParticlesGraphics : {
>		/** 给指定方块描框
>		 * @param {Player} player
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} r
>		 * @param {number} g
>		 * @param {number} b
>		 * @param {number} thickness
>		 * @param {number} time
>		 * @param {number} alpha
>		 */
>		DrawBlock(player,x,y,z,r,g,b,thickness,time,alpha) { (this.ParticlesGraphics_DrawBlock??=ll.import("PFLP", "ParticlesGraphics::DrawBlock"))(player,x,y,z,r,g,b,thickness,time,alpha)},
>		/** 给指定区域描框
>		 * @param {Player} player
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} r
>		 * @param {number} g
>		 * @param {number} b
>		 * @param {number} thickness
>		 * @param {number} time
>		 * @param {number} alpha
>		 */
>		DrawBorder(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha) { (this.ParticlesGraphics_DrawBorder??=ll.import("PFLP", "ParticlesGraphics::DrawBorder"))(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha)},
>	},
>	Lands : {
>		/** 检查指定立方体区域(float)是否有领地 返回值类型：bool
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		CheckCubeHasLand(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_CheckCubeHasLand??=ll.import("PFLP", "Lands::CheckCubeHasLand"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 检查指定立方体区域(int)是否有领地 返回值类型：bool
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		CheckCubeHasLandInt(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_CheckCubeHasLandInt??=ll.import("PFLP", "Lands::CheckCubeHasLandInt"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 检查指定坐标(float)是否有领地 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		CheckPosHasLand(x,y,z,dimensionId) { return (this.Lands_CheckPosHasLand??=ll.import("PFLP", "Lands::CheckPosHasLand"))(x,y,z,dimensionId)},
>		/** 检查指定坐标(int)是否有领地 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		CheckPosHasLandInt(x,y,z,dimensionId) { return (this.Lands_CheckPosHasLandInt??=ll.import("PFLP", "Lands::CheckPosHasLandInt"))(x,y,z,dimensionId)},
>		/** 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandByCube(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_GetLandByCube??=ll.import("PFLP", "Lands::GetLandByCube"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_GetLandByCubeInt??=ll.import("PFLP", "Lands::GetLandByCubeInt"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandByPos(x,y,z,dimensionId) { return (this.Lands_GetLandByPos??=ll.import("PFLP", "Lands::GetLandByPos"))(x,y,z,dimensionId)},
>		/** 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandByPosInt(x,y,z,dimensionId) { return (this.Lands_GetLandByPosInt??=ll.import("PFLP", "Lands::GetLandByPosInt"))(x,y,z,dimensionId)},
>		/** 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandInfoByCube(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_GetLandInfoByCube??=ll.import("PFLP", "Lands::GetLandInfoByCube"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandInfoByCubeInt(x1,y1,z1,x2,y2,z2,dimensionId) { return (this.Lands_GetLandInfoByCubeInt??=ll.import("PFLP", "Lands::GetLandInfoByCubeInt"))(x1,y1,z1,x2,y2,z2,dimensionId)},
>		/** 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandInfoByPos(x,y,z,dimensionId) { return (this.Lands_GetLandInfoByPos??=ll.import("PFLP", "Lands::GetLandInfoByPos"))(x,y,z,dimensionId)},
>		/** 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {string}
>		 */
>		GetLandInfoByPosInt(x,y,z,dimensionId) { return (this.Lands_GetLandInfoByPosInt??=ll.import("PFLP", "Lands::GetLandInfoByPosInt"))(x,y,z,dimensionId)},
>		/** 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} landinfo
>		 * @returns {boolean}
>		 */
>		SetLandInfoByPos(x,y,z,dimensionId,landinfo) { return (this.Lands_SetLandInfoByPos??=ll.import("PFLP", "Lands::SetLandInfoByPos"))(x,y,z,dimensionId,landinfo)},
>		/** 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} landinfo
>		 * @returns {boolean}
>		 */
>		SetLandInfoByPosInt(x,y,z,dimensionId,landinfo) { return (this.Lands_SetLandInfoByPosInt??=ll.import("PFLP", "Lands::SetLandInfoByPosInt"))(x,y,z,dimensionId,landinfo)},
>		/** 新建领地 返回值类型：bool
>		 * @param {number} x1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CreateLand2D(x1,z1,x2,z2,dimensionId,playerXuid) { return (this.Lands_CreateLand2D??=ll.import("PFLP", "Lands::CreateLand2D"))(x1,z1,x2,z2,dimensionId,playerXuid)},
>		/** 新建领地 返回值类型：bool
>		 * @param {number} x1
>		 * @param {number} y1
>		 * @param {number} z1
>		 * @param {number} x2
>		 * @param {number} y2
>		 * @param {number} z2
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CreateLand3D(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid) { return (this.Lands_CreateLand3D??=ll.import("PFLP", "Lands::CreateLand3D"))(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid)},
>		/** 删除指定坐标(float)的领地 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		DeleteLandByPos(x,y,z,dimensionId) { return (this.Lands_DeleteLandByPos??=ll.import("PFLP", "Lands::DeleteLandByPos"))(x,y,z,dimensionId)},
>		/** 删除指定坐标(int)的领地 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @returns {boolean}
>		 */
>		DeleteLandByPosInt(x,y,z,dimensionId) { return (this.Lands_DeleteLandByPosInt??=ll.import("PFLP", "Lands::DeleteLandByPosInt"))(x,y,z,dimensionId)},
>		/** 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetLandPermissionByPos(x,y,z,dimensionId,playerXuid) { return (this.Lands_GetLandPermissionByPos??=ll.import("PFLP", "Lands::GetLandPermissionByPos"))(x,y,z,dimensionId,playerXuid)},
>		/** 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {string}
>		 */
>		GetLandPermissionByPosInt(x,y,z,dimensionId,playerXuid) { return (this.Lands_GetLandPermissionByPosInt??=ll.import("PFLP", "Lands::GetLandPermissionByPosInt"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>		 * @param {string} permissionId
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckLandPermissionByPos(permissionId,x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckLandPermissionByPos??=ll.import("PFLP", "Lands::CheckLandPermissionByPos"))(permissionId,x,y,z,dimensionId,playerXuid)},
>		/** 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>		 * @param {string} permissionId
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckLandPermissionByPosInt(permissionId,x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckLandPermissionByPosInt??=ll.import("PFLP", "Lands::CheckLandPermissionByPosInt"))(permissionId,x,y,z,dimensionId,playerXuid)},
>		/** 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckPlayerIsLandOwnerByPos(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckPlayerIsLandOwnerByPos??=ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPos"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckPlayerIsLandOwnerByPosInt(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckPlayerIsLandOwnerByPosInt??=ll.import("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckIsLandSharedToPlayerByPos(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckIsLandSharedToPlayerByPos??=ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPos"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckIsLandSharedToPlayerByPosInt(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckIsLandSharedToPlayerByPosInt??=ll.import("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckPlayerHasCreateChestPermission(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckPlayerHasCreateChestPermission??=ll.import("PFLP", "Lands::CheckPlayerHasCreateChestPermission"))(x,y,z,dimensionId,playerXuid)},
>		/** 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>		 * @param {number} x
>		 * @param {number} y
>		 * @param {number} z
>		 * @param {number} dimensionId
>		 * @param {string} playerXuid
>		 * @returns {boolean}
>		 */
>		CheckPlayerHasOpenChestPermission(x,y,z,dimensionId,playerXuid) { return (this.Lands_CheckPlayerHasOpenChestPermission??=ll.import("PFLP", "Lands::CheckPlayerHasOpenChestPermission"))(x,y,z,dimensionId,playerXuid)},
>	},
>	Money : {
>		/** 获取玩家(指定玩家名)金钱 返回值类型：long
>		 * @param {string} playerXuid
>		 * @returns {number}
>		 */
>		Get(playerXuid) { return (this.Money_Get??=ll.import("PFLP", "Money::Get"))(playerXuid)},
>		/** 给玩家(指定玩家名)加钱
>		 * @param {string} playerXuid
>		 * @param {number} count
>		 * @param {string} info
>		 */
>		Add(playerXuid,count,info) { (this.Money_Add??=ll.import("PFLP", "Money::Add"))(playerXuid,count,info)},
>		/** 给玩家(指定玩家名)减钱
>		 * @param {string} playerXuid
>		 * @param {number} count
>		 * @param {string} info
>		 */
>		Remove(playerXuid,count,info) { (this.Money_Remove??=ll.import("PFLP", "Money::Remove"))(playerXuid,count,info)},
>	},
>};
>
>```
></details>
>
>---
>
</details>

<details>
<summary><b>All Api in C++ / 全部C++接口<b></summary>

``` C++
// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
auto General_SetConfig = RemoteCall::importAs<bool(std::string const& jsonStr)>("PFLP", "General::SetConfig");
// 获取全局配置文件（JSON字符串） 返回值类型：string
auto General_GetConfig = RemoteCall::importAs<std::string()>("PFLP", "General::GetConfig");
// 重新加载所有功能的配置文件
auto General_Reload = RemoteCall::importAs<void()>("PFLP", "General::Reload");
// 设置命令禁用(可设置提示)
auto Command_SetCommandDisabled = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& cmd,std::string const& feedback)>("PFLP", "Command::SetCommandDisabled");
// 设置命令启用
auto Command_SetCommandEnabled = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& cmd)>("PFLP", "Command::SetCommandEnabled");
// 翻译 返回值类型：string
auto Language_Translate = RemoteCall::importAs<std::string(std::string const& fromLanguage,std::string const& toLanguage,std::string const& text)>("PFLP", "Language::Translate");
// 设置玩家昵称
auto ChatEx_SetNickName = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& nickName)>("PFLP", "ChatEx::SetNickName");
// 设置玩家聊天时的名字
auto ChatEx_SetFakeName = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& fakeName)>("PFLP", "ChatEx::SetFakeName");
// 设置玩家聊天消息后缀
auto ChatEx_SetEnd = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& endStr)>("PFLP", "ChatEx::SetEnd");
// 设置玩家聊天消息前缀
auto ChatEx_SetStart = RemoteCall::importAs<void(std::string const& playerXuid,std::string const& startStr)>("PFLP", "ChatEx::SetStart");
// 获取玩家昵称 返回值类型：string
auto ChatEx_GetNickName = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetNickName");
// 获取玩家聊天时的名字 返回值类型：string
auto ChatEx_GetFakeName = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetFakeName");
// 获取玩家聊天消息后缀 返回值类型：string
auto ChatEx_GetEnd = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetEnd");
// 获取玩家聊天消息前缀 返回值类型：string
auto ChatEx_GetStart = RemoteCall::importAs<std::string(std::string const& playerXuid)>("PFLP", "ChatEx::GetStart");
// 给指定方块描框
auto ParticlesGraphics_DrawBlock = RemoteCall::importAs<void(Player& const& player,int const& x,int const& y,int const& z,float const& r,float const& g,float const& b,float const& thickness,float const& time,float const& alpha)>("PFLP", "ParticlesGraphics::DrawBlock");
// 给指定区域描框
auto ParticlesGraphics_DrawBorder = RemoteCall::importAs<void(Player& const& player,int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,float const& r,float const& g,float const& b,float const& thickness,float const& time,float const& alpha)>("PFLP", "ParticlesGraphics::DrawBorder");
// 检查指定立方体区域(float)是否有领地 返回值类型：bool
auto Lands_CheckCubeHasLand = RemoteCall::importAs<bool(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::CheckCubeHasLand");
// 检查指定立方体区域(int)是否有领地 返回值类型：bool
auto Lands_CheckCubeHasLandInt = RemoteCall::importAs<bool(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::CheckCubeHasLandInt");
// 检查指定坐标(float)是否有领地 返回值类型：bool
auto Lands_CheckPosHasLand = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::CheckPosHasLand");
// 检查指定坐标(int)是否有领地 返回值类型：bool
auto Lands_CheckPosHasLandInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::CheckPosHasLandInt");
// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandByCube = RemoteCall::importAs<std::string(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandByCube");
// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandByCubeInt = RemoteCall::importAs<std::string(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandByCubeInt");
// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::GetLandByPos");
// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::GetLandByPosInt");
// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandInfoByCube = RemoteCall::importAs<std::string(float const& x1,float const& y1,float const& z1,float const& x2,float const& y2,float const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByCube");
// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandInfoByCubeInt = RemoteCall::importAs<std::string(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByCubeInt");
// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandInfoByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByPos");
// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
auto Lands_GetLandInfoByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::GetLandInfoByPosInt");
// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
auto Lands_SetLandInfoByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& landinfo)>("PFLP", "Lands::SetLandInfoByPos");
// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
auto Lands_SetLandInfoByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& landinfo)>("PFLP", "Lands::SetLandInfoByPosInt");
// 新建领地 返回值类型：bool
auto Lands_CreateLand2D = RemoteCall::importAs<bool(int const& x1,int const& z1,int const& x2,int const& z2,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CreateLand2D");
// 新建领地 返回值类型：bool
auto Lands_CreateLand3D = RemoteCall::importAs<bool(int const& x1,int const& y1,int const& z1,int const& x2,int const& y2,int const& z2,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CreateLand3D");
// 删除指定坐标(float)的领地 返回值类型：bool
auto Lands_DeleteLandByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId)>("PFLP", "Lands::DeleteLandByPos");
// 删除指定坐标(int)的领地 返回值类型：bool
auto Lands_DeleteLandByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId)>("PFLP", "Lands::DeleteLandByPosInt");
// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
auto Lands_GetLandPermissionByPos = RemoteCall::importAs<std::string(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::GetLandPermissionByPos");
// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
auto Lands_GetLandPermissionByPosInt = RemoteCall::importAs<std::string(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::GetLandPermissionByPosInt");
// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
auto Lands_CheckLandPermissionByPos = RemoteCall::importAs<bool(std::string const& permissionId,float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckLandPermissionByPos");
// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
auto Lands_CheckLandPermissionByPosInt = RemoteCall::importAs<bool(std::string const& permissionId,int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckLandPermissionByPosInt");
// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
auto Lands_CheckPlayerIsLandOwnerByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
auto Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
auto Lands_CheckIsLandSharedToPlayerByPos = RemoteCall::importAs<bool(float const& x,float const& y,float const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
auto Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
auto Lands_CheckPlayerHasCreateChestPermission = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
auto Lands_CheckPlayerHasOpenChestPermission = RemoteCall::importAs<bool(int const& x,int const& y,int const& z,int const& dimensionId,std::string const& playerXuid)>("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
// 获取玩家(指定玩家名)金钱 返回值类型：long
auto Money_Get = RemoteCall::importAs<long long(std::string const& playerXuid)>("PFLP", "Money::Get");
// 给玩家(指定玩家名)加钱
auto Money_Add = RemoteCall::importAs<void(std::string const& playerXuid,long long const& count,std::string const& info)>("PFLP", "Money::Add");
// 给玩家(指定玩家名)减钱
auto Money_Remove = RemoteCall::importAs<void(std::string const& playerXuid,long long const& count,std::string const& info)>("PFLP", "Money::Remove");

```
</details>


<details><summary><b>All Api in C# /  C#全部接口<b></summary>

>---
><details><summary>C# imports / 直接导入</summary>
>
>``` C#
>using RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI;
>
>// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>var General_SetConfig = RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig");
>// 获取全局配置文件（JSON字符串） 返回值类型：string
>var General_GetConfig = RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig");
>// 重新加载所有功能的配置文件
>var General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload");
>// 设置命令禁用(可设置提示)
>var Command_SetCommandDisabled = RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled");
>// 设置命令启用
>var Command_SetCommandEnabled = RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled");
>// 翻译 返回值类型：string
>var Language_Translate = RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate");
>// 设置玩家昵称
>var ChatEx_SetNickName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName");
>// 设置玩家聊天时的名字
>var ChatEx_SetFakeName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName");
>// 设置玩家聊天消息后缀
>var ChatEx_SetEnd = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd");
>// 设置玩家聊天消息前缀
>var ChatEx_SetStart = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart");
>// 获取玩家昵称 返回值类型：string
>var ChatEx_GetNickName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName");
>// 获取玩家聊天时的名字 返回值类型：string
>var ChatEx_GetFakeName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName");
>// 获取玩家聊天消息后缀 返回值类型：string
>var ChatEx_GetEnd = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd");
>// 获取玩家聊天消息前缀 返回值类型：string
>var ChatEx_GetStart = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart");
>// 给指定方块描框
>var ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As<Player,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock");
>// 给指定区域描框
>var ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As<Player,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder");
>// 检查指定立方体区域(float)是否有领地 返回值类型：bool
>var Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand");
>// 检查指定立方体区域(int)是否有领地 返回值类型：bool
>var Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt");
>// 检查指定坐标(float)是否有领地 返回值类型：bool
>var Lands_CheckPosHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand");
>// 检查指定坐标(int)是否有领地 返回值类型：bool
>var Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt");
>// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube");
>// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt");
>// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos");
>// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt");
>// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube");
>// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt");
>// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos");
>// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>var Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt");
>// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>var Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos");
>// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>var Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt");
>// 新建领地 返回值类型：bool
>var Lands_CreateLand2D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D");
>// 新建领地 返回值类型：bool
>var Lands_CreateLand3D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D");
>// 删除指定坐标(float)的领地 返回值类型：bool
>var Lands_DeleteLandByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos");
>// 删除指定坐标(int)的领地 返回值类型：bool
>var Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt");
>// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>var Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos");
>// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>var Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt");
>// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>var Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos");
>// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>var Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt");
>// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>var Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos");
>// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>var Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt");
>// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>var Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos");
>// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>var Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt");
>// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>var Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission");
>// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>var Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission");
>// 获取玩家(指定玩家名)金钱 返回值类型：long
>var Money_Get = RemoteCallAPI.ImportAs<long,string>("PFLP", "Money::Get");
>// 给玩家(指定玩家名)加钱
>var Money_Add = RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Add");
>// 给玩家(指定玩家名)减钱
>var Money_Remove = RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Remove");
>
>```
></details>
><details><summary>C# class / C#静态类定义（推荐）</summary>
>
>``` C# 
>using RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI;
>
>internal static class PFLP {
>	public static class General {
>		private static Lazy<RemoteCallHandler_1<bool,string>>  General_SetConfig_instance = new(()=> RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig"));
>		/// <summary> 设置全局配置文件（要求JSON字符串） 返回值类型：bool </summary>
>		public static bool SetConfig(string jsonStr) {
>			return General_SetConfig_instance.Value(jsonStr);
>		}
>		private static Lazy<RemoteCallHandler_0<string>>  General_GetConfig_instance = new(()=> RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig"));
>		/// <summary> 获取全局配置文件（JSON字符串） 返回值类型：string </summary>
>		public static string GetConfig() {
>			return General_GetConfig_instance.Value();
>		}
>		private static Lazy<RemoteCallHandler_void_0>  General_Reload_instance = new(()=> RemoteCallAPI.Import_As("PFLP", "General::Reload"));
>		/// <summary> 重新加载所有功能的配置文件 </summary>
>		public static void Reload() {
>			General_Reload_instance.Value();
>		}
>	}
>	public static class Command {
>		private static Lazy<RemoteCallHandler_void_3<string,string,string>>  Command_SetCommandDisabled_instance = new(()=> RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled"));
>		/// <summary> 设置命令禁用(可设置提示) </summary>
>		public static void SetCommandDisabled(string playerXuid,string cmd,string feedback) {
>			Command_SetCommandDisabled_instance.Value(playerXuid,cmd,feedback);
>		}
>		private static Lazy<RemoteCallHandler_void_2<string,string>>  Command_SetCommandEnabled_instance = new(()=> RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled"));
>		/// <summary> 设置命令启用 </summary>
>		public static void SetCommandEnabled(string playerXuid,string cmd) {
>			Command_SetCommandEnabled_instance.Value(playerXuid,cmd);
>		}
>	}
>	public static class Language {
>		private static Lazy<RemoteCallHandler_3<string,string,string,string>>  Language_Translate_instance = new(()=> RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate"));
>		/// <summary> 翻译 返回值类型：string </summary>
>		public static string Translate(string fromLanguage,string toLanguage,string text) {
>			return Language_Translate_instance.Value(fromLanguage,toLanguage,text);
>		}
>	}
>	public static class ChatEx {
>		private static Lazy<RemoteCallHandler_void_2<string,string>>  ChatEx_SetNickName_instance = new(()=> RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName"));
>		/// <summary> 设置玩家昵称 </summary>
>		public static void SetNickName(string playerXuid,string nickName) {
>			ChatEx_SetNickName_instance.Value(playerXuid,nickName);
>		}
>		private static Lazy<RemoteCallHandler_void_2<string,string>>  ChatEx_SetFakeName_instance = new(()=> RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName"));
>		/// <summary> 设置玩家聊天时的名字 </summary>
>		public static void SetFakeName(string playerXuid,string fakeName) {
>			ChatEx_SetFakeName_instance.Value(playerXuid,fakeName);
>		}
>		private static Lazy<RemoteCallHandler_void_2<string,string>>  ChatEx_SetEnd_instance = new(()=> RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd"));
>		/// <summary> 设置玩家聊天消息后缀 </summary>
>		public static void SetEnd(string playerXuid,string endStr) {
>			ChatEx_SetEnd_instance.Value(playerXuid,endStr);
>		}
>		private static Lazy<RemoteCallHandler_void_2<string,string>>  ChatEx_SetStart_instance = new(()=> RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart"));
>		/// <summary> 设置玩家聊天消息前缀 </summary>
>		public static void SetStart(string playerXuid,string startStr) {
>			ChatEx_SetStart_instance.Value(playerXuid,startStr);
>		}
>		private static Lazy<RemoteCallHandler_1<string,string>>  ChatEx_GetNickName_instance = new(()=> RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName"));
>		/// <summary> 获取玩家昵称 返回值类型：string </summary>
>		public static string GetNickName(string playerXuid) {
>			return ChatEx_GetNickName_instance.Value(playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_1<string,string>>  ChatEx_GetFakeName_instance = new(()=> RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName"));
>		/// <summary> 获取玩家聊天时的名字 返回值类型：string </summary>
>		public static string GetFakeName(string playerXuid) {
>			return ChatEx_GetFakeName_instance.Value(playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_1<string,string>>  ChatEx_GetEnd_instance = new(()=> RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd"));
>		/// <summary> 获取玩家聊天消息后缀 返回值类型：string </summary>
>		public static string GetEnd(string playerXuid) {
>			return ChatEx_GetEnd_instance.Value(playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_1<string,string>>  ChatEx_GetStart_instance = new(()=> RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart"));
>		/// <summary> 获取玩家聊天消息前缀 返回值类型：string </summary>
>		public static string GetStart(string playerXuid) {
>			return ChatEx_GetStart_instance.Value(playerXuid);
>		}
>	}
>	public static class ParticlesGraphics {
>		private static Lazy<RemoteCallHandler_void_10<Player,int,int,int,float,float,float,float,float,float>>  ParticlesGraphics_DrawBlock_instance = new(()=> RemoteCallAPI.Import_As<Player,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock"));
>		/// <summary> 给指定方块描框 </summary>
>		public static void DrawBlock(Player player,int x,int y,int z,float r,float g,float b,float thickness,float time,float alpha) {
>			ParticlesGraphics_DrawBlock_instance.Value(player,x,y,z,r,g,b,thickness,time,alpha);
>		}
>		private static Lazy<RemoteCallHandler_void_13<Player,int,int,int,int,int,int,float,float,float,float,float,float>>  ParticlesGraphics_DrawBorder_instance = new(()=> RemoteCallAPI.Import_As<Player,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder"));
>		/// <summary> 给指定区域描框 </summary>
>		public static void DrawBorder(Player player,int x1,int y1,int z1,int x2,int y2,int z2,float r,float g,float b,float thickness,float time,float alpha) {
>			ParticlesGraphics_DrawBorder_instance.Value(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha);
>		}
>	}
>	public static class Lands {
>		private static Lazy<RemoteCallHandler_7<bool,float,float,float,float,float,float,int>>  Lands_CheckCubeHasLand_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand"));
>		/// <summary> 检查指定立方体区域(float)是否有领地 返回值类型：bool </summary>
>		public static bool CheckCubeHasLand(float x1,float y1,float z1,float x2,float y2,float z2,int dimensionId) {
>			return Lands_CheckCubeHasLand_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_7<bool,int,int,int,int,int,int,int>>  Lands_CheckCubeHasLandInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt"));
>		/// <summary> 检查指定立方体区域(int)是否有领地 返回值类型：bool </summary>
>		public static bool CheckCubeHasLandInt(int x1,int y1,int z1,int x2,int y2,int z2,int dimensionId) {
>			return Lands_CheckCubeHasLandInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<bool,float,float,float,int>>  Lands_CheckPosHasLand_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand"));
>		/// <summary> 检查指定坐标(float)是否有领地 返回值类型：bool </summary>
>		public static bool CheckPosHasLand(float x,float y,float z,int dimensionId) {
>			return Lands_CheckPosHasLand_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<bool,int,int,int,int>>  Lands_CheckPosHasLandInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt"));
>		/// <summary> 检查指定坐标(int)是否有领地 返回值类型：bool </summary>
>		public static bool CheckPosHasLandInt(int x,int y,int z,int dimensionId) {
>			return Lands_CheckPosHasLandInt_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_7<string,float,float,float,float,float,float,int>>  Lands_GetLandByCube_instance = new(()=> RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube"));
>		/// <summary> 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandByCube(float x1,float y1,float z1,float x2,float y2,float z2,int dimensionId) {
>			return Lands_GetLandByCube_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_7<string,int,int,int,int,int,int,int>>  Lands_GetLandByCubeInt_instance = new(()=> RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt"));
>		/// <summary> 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandByCubeInt(int x1,int y1,int z1,int x2,int y2,int z2,int dimensionId) {
>			return Lands_GetLandByCubeInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<string,float,float,float,int>>  Lands_GetLandByPos_instance = new(()=> RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos"));
>		/// <summary> 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandByPos(float x,float y,float z,int dimensionId) {
>			return Lands_GetLandByPos_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<string,int,int,int,int>>  Lands_GetLandByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt"));
>		/// <summary> 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandByPosInt(int x,int y,int z,int dimensionId) {
>			return Lands_GetLandByPosInt_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_7<string,float,float,float,float,float,float,int>>  Lands_GetLandInfoByCube_instance = new(()=> RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube"));
>		/// <summary> 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandInfoByCube(float x1,float y1,float z1,float x2,float y2,float z2,int dimensionId) {
>			return Lands_GetLandInfoByCube_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_7<string,int,int,int,int,int,int,int>>  Lands_GetLandInfoByCubeInt_instance = new(()=> RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt"));
>		/// <summary> 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandInfoByCubeInt(int x1,int y1,int z1,int x2,int y2,int z2,int dimensionId) {
>			return Lands_GetLandInfoByCubeInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<string,float,float,float,int>>  Lands_GetLandInfoByPos_instance = new(()=> RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos"));
>		/// <summary> 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandInfoByPos(float x,float y,float z,int dimensionId) {
>			return Lands_GetLandInfoByPos_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<string,int,int,int,int>>  Lands_GetLandInfoByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt"));
>		/// <summary> 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		public static string GetLandInfoByPosInt(int x,int y,int z,int dimensionId) {
>			return Lands_GetLandInfoByPosInt_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,float,float,float,int,string>>  Lands_SetLandInfoByPos_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos"));
>		/// <summary> 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>		public static bool SetLandInfoByPos(float x,float y,float z,int dimensionId,string landinfo) {
>			return Lands_SetLandInfoByPos_instance.Value(x,y,z,dimensionId,landinfo);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,int,int,int,int,string>>  Lands_SetLandInfoByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt"));
>		/// <summary> 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>		public static bool SetLandInfoByPosInt(int x,int y,int z,int dimensionId,string landinfo) {
>			return Lands_SetLandInfoByPosInt_instance.Value(x,y,z,dimensionId,landinfo);
>		}
>		private static Lazy<RemoteCallHandler_6<bool,int,int,int,int,int,string>>  Lands_CreateLand2D_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D"));
>		/// <summary> 新建领地 返回值类型：bool </summary>
>		public static bool CreateLand2D(int x1,int z1,int x2,int z2,int dimensionId,string playerXuid) {
>			return Lands_CreateLand2D_instance.Value(x1,z1,x2,z2,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_8<bool,int,int,int,int,int,int,int,string>>  Lands_CreateLand3D_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D"));
>		/// <summary> 新建领地 返回值类型：bool </summary>
>		public static bool CreateLand3D(int x1,int y1,int z1,int x2,int y2,int z2,int dimensionId,string playerXuid) {
>			return Lands_CreateLand3D_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_4<bool,float,float,float,int>>  Lands_DeleteLandByPos_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos"));
>		/// <summary> 删除指定坐标(float)的领地 返回值类型：bool </summary>
>		public static bool DeleteLandByPos(float x,float y,float z,int dimensionId) {
>			return Lands_DeleteLandByPos_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_4<bool,int,int,int,int>>  Lands_DeleteLandByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt"));
>		/// <summary> 删除指定坐标(int)的领地 返回值类型：bool </summary>
>		public static bool DeleteLandByPosInt(int x,int y,int z,int dimensionId) {
>			return Lands_DeleteLandByPosInt_instance.Value(x,y,z,dimensionId);
>		}
>		private static Lazy<RemoteCallHandler_5<string,float,float,float,int,string>>  Lands_GetLandPermissionByPos_instance = new(()=> RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos"));
>		/// <summary> 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>		public static string GetLandPermissionByPos(float x,float y,float z,int dimensionId,string playerXuid) {
>			return Lands_GetLandPermissionByPos_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<string,int,int,int,int,string>>  Lands_GetLandPermissionByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt"));
>		/// <summary> 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>		public static string GetLandPermissionByPosInt(int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_GetLandPermissionByPosInt_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_6<bool,string,float,float,float,int,string>>  Lands_CheckLandPermissionByPos_instance = new(()=> RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos"));
>		/// <summary> 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>		public static bool CheckLandPermissionByPos(string permissionId,float x,float y,float z,int dimensionId,string playerXuid) {
>			return Lands_CheckLandPermissionByPos_instance.Value(permissionId,x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_6<bool,string,int,int,int,int,string>>  Lands_CheckLandPermissionByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt"));
>		/// <summary> 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>		public static bool CheckLandPermissionByPosInt(string permissionId,int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_CheckLandPermissionByPosInt_instance.Value(permissionId,x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,float,float,float,int,string>>  Lands_CheckPlayerIsLandOwnerByPos_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos"));
>		/// <summary> 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool </summary>
>		public static bool CheckPlayerIsLandOwnerByPos(float x,float y,float z,int dimensionId,string playerXuid) {
>			return Lands_CheckPlayerIsLandOwnerByPos_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,int,int,int,int,string>>  Lands_CheckPlayerIsLandOwnerByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt"));
>		/// <summary> 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool </summary>
>		public static bool CheckPlayerIsLandOwnerByPosInt(int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_CheckPlayerIsLandOwnerByPosInt_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,float,float,float,int,string>>  Lands_CheckIsLandSharedToPlayerByPos_instance = new(()=> RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos"));
>		/// <summary> 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>		public static bool CheckIsLandSharedToPlayerByPos(float x,float y,float z,int dimensionId,string playerXuid) {
>			return Lands_CheckIsLandSharedToPlayerByPos_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,int,int,int,int,string>>  Lands_CheckIsLandSharedToPlayerByPosInt_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt"));
>		/// <summary> 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>		public static bool CheckIsLandSharedToPlayerByPosInt(int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_CheckIsLandSharedToPlayerByPosInt_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,int,int,int,int,string>>  Lands_CheckPlayerHasCreateChestPermission_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission"));
>		/// <summary> 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>		public static bool CheckPlayerHasCreateChestPermission(int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_CheckPlayerHasCreateChestPermission_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_5<bool,int,int,int,int,string>>  Lands_CheckPlayerHasOpenChestPermission_instance = new(()=> RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission"));
>		/// <summary> 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>		public static bool CheckPlayerHasOpenChestPermission(int x,int y,int z,int dimensionId,string playerXuid) {
>			return Lands_CheckPlayerHasOpenChestPermission_instance.Value(x,y,z,dimensionId,playerXuid);
>		}
>	}
>	public static class Money {
>		private static Lazy<RemoteCallHandler_1<long,string>>  Money_Get_instance = new(()=> RemoteCallAPI.ImportAs<long,string>("PFLP", "Money::Get"));
>		/// <summary> 获取玩家(指定玩家名)金钱 返回值类型：long </summary>
>		public static long Get(string playerXuid) {
>			return Money_Get_instance.Value(playerXuid);
>		}
>		private static Lazy<RemoteCallHandler_void_3<string,long,string>>  Money_Add_instance = new(()=> RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Add"));
>		/// <summary> 给玩家(指定玩家名)加钱 </summary>
>		public static void Add(string playerXuid,long count,string info) {
>			Money_Add_instance.Value(playerXuid,count,info);
>		}
>		private static Lazy<RemoteCallHandler_void_3<string,long,string>>  Money_Remove_instance = new(()=> RemoteCallAPI.Import_As<string,long,string>("PFLP", "Money::Remove"));
>		/// <summary> 给玩家(指定玩家名)减钱 </summary>
>		public static void Remove(string playerXuid,long count,string info) {
>			Money_Remove_instance.Value(playerXuid,count,info);
>		}
>	}
>}
> 
>```
></details>
>
>---
>
</details>


<details><summary><b>All Api in Visual Basic .Net / VB接口汇总<b></summary>


>---
><details><summary>VB imports / 直接导入</summary>
>
>``` VB
>Imports RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI;
>
>' 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>Dim General_SetConfig = RemoteCallAPI.ImportAs(Of Boolean,String)("PFLP", "General::SetConfig")
>' 获取全局配置文件（JSON字符串） 返回值类型：string
>Dim General_GetConfig = RemoteCallAPI.ImportAs(Of String)("PFLP", "General::GetConfig")
>' 重新加载所有功能的配置文件
>Dim General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload")
>' 设置命令禁用(可设置提示)
>Dim Command_SetCommandDisabled = RemoteCallAPI.Import_As(Of String,String,String)("PFLP", "Command::SetCommandDisabled")
>' 设置命令启用
>Dim Command_SetCommandEnabled = RemoteCallAPI.Import_As(Of String,String)("PFLP", "Command::SetCommandEnabled")
>' 翻译 返回值类型：string
>Dim Language_Translate = RemoteCallAPI.ImportAs(Of String,String,String,String)("PFLP", "Language::Translate")
>' 设置玩家昵称
>Dim ChatEx_SetNickName = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetNickName")
>' 设置玩家聊天时的名字
>Dim ChatEx_SetFakeName = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetFakeName")
>' 设置玩家聊天消息后缀
>Dim ChatEx_SetEnd = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetEnd")
>' 设置玩家聊天消息前缀
>Dim ChatEx_SetStart = RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetStart")
>' 获取玩家昵称 返回值类型：string
>Dim ChatEx_GetNickName = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetNickName")
>' 获取玩家聊天时的名字 返回值类型：string
>Dim ChatEx_GetFakeName = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetFakeName")
>' 获取玩家聊天消息后缀 返回值类型：string
>Dim ChatEx_GetEnd = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetEnd")
>' 获取玩家聊天消息前缀 返回值类型：string
>Dim ChatEx_GetStart = RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetStart")
>' 给指定方块描框
>Dim ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBlock")
>' 给指定区域描框
>Dim ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBorder")
>' 检查指定立方体区域(float)是否有领地 返回值类型：bool
>Dim Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::CheckCubeHasLand")
>' 检查指定立方体区域(int)是否有领地 返回值类型：bool
>Dim Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckCubeHasLandInt")
>' 检查指定坐标(float)是否有领地 返回值类型：bool
>Dim Lands_CheckPosHasLand = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::CheckPosHasLand")
>' 检查指定坐标(int)是否有领地 返回值类型：bool
>Dim Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckPosHasLandInt")
>' 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByCube = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByCube")
>' 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByCubeInt")
>' 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByPos")
>' 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByPosInt")
>' 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByCube")
>' 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByCubeInt")
>' 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByPos")
>' 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>Dim Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByPosInt")
>' 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>Dim Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::SetLandInfoByPos")
>' 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>Dim Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::SetLandInfoByPosInt")
>' 新建领地 返回值类型：bool
>Dim Lands_CreateLand2D = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand2D")
>' 新建领地 返回值类型：bool
>Dim Lands_CreateLand3D = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand3D")
>' 删除指定坐标(float)的领地 返回值类型：bool
>Dim Lands_DeleteLandByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::DeleteLandByPos")
>' 删除指定坐标(int)的领地 返回值类型：bool
>Dim Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::DeleteLandByPosInt")
>' 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>Dim Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer,String)("PFLP", "Lands::GetLandPermissionByPos")
>' 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>Dim Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::GetLandPermissionByPosInt")
>' 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>Dim Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs(Of Boolean,String,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckLandPermissionByPos")
>' 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>Dim Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs(Of Boolean,String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckLandPermissionByPosInt")
>' 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>Dim Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPos")
>' 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>Dim Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt")
>' 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>Dim Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPos")
>' 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>Dim Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt")
>' 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>Dim Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasCreateChestPermission")
>' 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>Dim Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasOpenChestPermission")
>' 获取玩家(指定玩家名)金钱 返回值类型：long
>Dim Money_Get = RemoteCallAPI.ImportAs(Of Long,String)("PFLP", "Money::Get")
>' 给玩家(指定玩家名)加钱
>Dim Money_Add = RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Add")
>' 给玩家(指定玩家名)减钱
>Dim Money_Remove = RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Remove")
>
>```
></details>
><details><summary>VB Module / 模块类定义（推荐）</summary>
>
>``` VB 
>Imports RemoteCallAPI = LiteLoader.RemoteCall.RemoteCallAPI;
>
>Friend Module PFLP
>	Public NotInheritable Class General
>		Private Shared General_SetConfig_instance As Lazy(Of RemoteCallHandler_1(Of Boolean,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,String)("PFLP", "General::SetConfig"))
>		''' <summary> 设置全局配置文件（要求JSON字符串） 返回值类型：bool </summary>
>		Public Shared Function SetConfig(jsonStr As String) As bool 
>			Return General_SetConfig_instance.Value(jsonStr)
>		End Function
>		Private Shared General_GetConfig_instance As Lazy(Of RemoteCallHandler_0(Of String))(Function() RemoteCallAPI.ImportAs(Of String)("PFLP", "General::GetConfig"))
>		''' <summary> 获取全局配置文件（JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetConfig() As string 
>			Return General_GetConfig_instance.Value()
>		End Function
>		Private Shared General_Reload_instance As Lazy(Of RemoteCallHandler_void_0)(Function() RemoteCallAPI.Import_As("PFLP", "General::Reload"))
>		''' <summary> 重新加载所有功能的配置文件 </summary>
>		Public Shared Sub Reload()  
>			General_Reload_instance.Value()
>		End Sub
>	End Class
>	Public NotInheritable Class Command
>		Private Shared Command_SetCommandDisabled_instance As Lazy(Of RemoteCallHandler_void_3(Of String,String,String))(Function() RemoteCallAPI.Import_As(Of String,String,String)("PFLP", "Command::SetCommandDisabled"))
>		''' <summary> 设置命令禁用(可设置提示) </summary>
>		Public Shared Sub SetCommandDisabled(playerXuid As String,cmd As String,feedback As String)  
>			Command_SetCommandDisabled_instance.Value(playerXuid,cmd,feedback)
>		End Sub
>		Private Shared Command_SetCommandEnabled_instance As Lazy(Of RemoteCallHandler_void_2(Of String,String))(Function() RemoteCallAPI.Import_As(Of String,String)("PFLP", "Command::SetCommandEnabled"))
>		''' <summary> 设置命令启用 </summary>
>		Public Shared Sub SetCommandEnabled(playerXuid As String,cmd As String)  
>			Command_SetCommandEnabled_instance.Value(playerXuid,cmd)
>		End Sub
>	End Class
>	Public NotInheritable Class Language
>		Private Shared Language_Translate_instance As Lazy(Of RemoteCallHandler_3(Of String,String,String,String))(Function() RemoteCallAPI.ImportAs(Of String,String,String,String)("PFLP", "Language::Translate"))
>		''' <summary> 翻译 返回值类型：string </summary>
>		Public Shared Function Translate(fromLanguage As String,toLanguage As String,text As String) As string 
>			Return Language_Translate_instance.Value(fromLanguage,toLanguage,text)
>		End Function
>	End Class
>	Public NotInheritable Class ChatEx
>		Private Shared ChatEx_SetNickName_instance As Lazy(Of RemoteCallHandler_void_2(Of String,String))(Function() RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetNickName"))
>		''' <summary> 设置玩家昵称 </summary>
>		Public Shared Sub SetNickName(playerXuid As String,nickName As String)  
>			ChatEx_SetNickName_instance.Value(playerXuid,nickName)
>		End Sub
>		Private Shared ChatEx_SetFakeName_instance As Lazy(Of RemoteCallHandler_void_2(Of String,String))(Function() RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetFakeName"))
>		''' <summary> 设置玩家聊天时的名字 </summary>
>		Public Shared Sub SetFakeName(playerXuid As String,fakeName As String)  
>			ChatEx_SetFakeName_instance.Value(playerXuid,fakeName)
>		End Sub
>		Private Shared ChatEx_SetEnd_instance As Lazy(Of RemoteCallHandler_void_2(Of String,String))(Function() RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetEnd"))
>		''' <summary> 设置玩家聊天消息后缀 </summary>
>		Public Shared Sub SetEnd(playerXuid As String,endStr As String)  
>			ChatEx_SetEnd_instance.Value(playerXuid,endStr)
>		End Sub
>		Private Shared ChatEx_SetStart_instance As Lazy(Of RemoteCallHandler_void_2(Of String,String))(Function() RemoteCallAPI.Import_As(Of String,String)("PFLP", "ChatEx::SetStart"))
>		''' <summary> 设置玩家聊天消息前缀 </summary>
>		Public Shared Sub SetStart(playerXuid As String,startStr As String)  
>			ChatEx_SetStart_instance.Value(playerXuid,startStr)
>		End Sub
>		Private Shared ChatEx_GetNickName_instance As Lazy(Of RemoteCallHandler_1(Of String,String))(Function() RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetNickName"))
>		''' <summary> 获取玩家昵称 返回值类型：string </summary>
>		Public Shared Function GetNickName(playerXuid As String) As string 
>			Return ChatEx_GetNickName_instance.Value(playerXuid)
>		End Function
>		Private Shared ChatEx_GetFakeName_instance As Lazy(Of RemoteCallHandler_1(Of String,String))(Function() RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetFakeName"))
>		''' <summary> 获取玩家聊天时的名字 返回值类型：string </summary>
>		Public Shared Function GetFakeName(playerXuid As String) As string 
>			Return ChatEx_GetFakeName_instance.Value(playerXuid)
>		End Function
>		Private Shared ChatEx_GetEnd_instance As Lazy(Of RemoteCallHandler_1(Of String,String))(Function() RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetEnd"))
>		''' <summary> 获取玩家聊天消息后缀 返回值类型：string </summary>
>		Public Shared Function GetEnd(playerXuid As String) As string 
>			Return ChatEx_GetEnd_instance.Value(playerXuid)
>		End Function
>		Private Shared ChatEx_GetStart_instance As Lazy(Of RemoteCallHandler_1(Of String,String))(Function() RemoteCallAPI.ImportAs(Of String,String)("PFLP", "ChatEx::GetStart"))
>		''' <summary> 获取玩家聊天消息前缀 返回值类型：string </summary>
>		Public Shared Function GetStart(playerXuid As String) As string 
>			Return ChatEx_GetStart_instance.Value(playerXuid)
>		End Function
>	End Class
>	Public NotInheritable Class ParticlesGraphics
>		Private Shared ParticlesGraphics_DrawBlock_instance As Lazy(Of RemoteCallHandler_void_10(Of IntPtr,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single))(Function() RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBlock"))
>		''' <summary> 给指定方块描框 </summary>
>		Public Shared Sub DrawBlock(player As IntPtr,x As Integer,y As Integer,z As Integer,r As Single,g As Single,b As Single,thickness As Single,time As Single,alpha As Single)  
>			ParticlesGraphics_DrawBlock_instance.Value(player,x,y,z,r,g,b,thickness,time,alpha)
>		End Sub
>		Private Shared ParticlesGraphics_DrawBorder_instance As Lazy(Of RemoteCallHandler_void_13(Of IntPtr,Integer,Integer,Integer,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single))(Function() RemoteCallAPI.Import_As(Of IntPtr,Integer,Integer,Integer,Integer,Integer,Integer,Single,Single,Single,Single,Single,Single)("PFLP", "ParticlesGraphics::DrawBorder"))
>		''' <summary> 给指定区域描框 </summary>
>		Public Shared Sub DrawBorder(player As IntPtr,x1 As Integer,y1 As Integer,z1 As Integer,x2 As Integer,y2 As Integer,z2 As Integer,r As Single,g As Single,b As Single,thickness As Single,time As Single,alpha As Single)  
>			ParticlesGraphics_DrawBorder_instance.Value(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha)
>		End Sub
>	End Class
>	Public NotInheritable Class Lands
>		Private Shared Lands_CheckCubeHasLand_instance As Lazy(Of RemoteCallHandler_7(Of Boolean,Single,Single,Single,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::CheckCubeHasLand"))
>		''' <summary> 检查指定立方体区域(float)是否有领地 返回值类型：bool </summary>
>		Public Shared Function CheckCubeHasLand(x1 As Single,y1 As Single,z1 As Single,x2 As Single,y2 As Single,z2 As Single,dimensionId As Integer) As bool 
>			Return Lands_CheckCubeHasLand_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_CheckCubeHasLandInt_instance As Lazy(Of RemoteCallHandler_7(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckCubeHasLandInt"))
>		''' <summary> 检查指定立方体区域(int)是否有领地 返回值类型：bool </summary>
>		Public Shared Function CheckCubeHasLandInt(x1 As Integer,y1 As Integer,z1 As Integer,x2 As Integer,y2 As Integer,z2 As Integer,dimensionId As Integer) As bool 
>			Return Lands_CheckCubeHasLandInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_CheckPosHasLand_instance As Lazy(Of RemoteCallHandler_4(Of Boolean,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::CheckPosHasLand"))
>		''' <summary> 检查指定坐标(float)是否有领地 返回值类型：bool </summary>
>		Public Shared Function CheckPosHasLand(x As Single,y As Single,z As Single,dimensionId As Integer) As bool 
>			Return Lands_CheckPosHasLand_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_CheckPosHasLandInt_instance As Lazy(Of RemoteCallHandler_4(Of Boolean,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::CheckPosHasLandInt"))
>		''' <summary> 检查指定坐标(int)是否有领地 返回值类型：bool </summary>
>		Public Shared Function CheckPosHasLandInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer) As bool 
>			Return Lands_CheckPosHasLandInt_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_GetLandByCube_instance As Lazy(Of RemoteCallHandler_7(Of String,Single,Single,Single,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByCube"))
>		''' <summary> 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandByCube(x1 As Single,y1 As Single,z1 As Single,x2 As Single,y2 As Single,z2 As Single,dimensionId As Integer) As string 
>			Return Lands_GetLandByCube_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_GetLandByCubeInt_instance As Lazy(Of RemoteCallHandler_7(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByCubeInt"))
>		''' <summary> 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandByCubeInt(x1 As Integer,y1 As Integer,z1 As Integer,x2 As Integer,y2 As Integer,z2 As Integer,dimensionId As Integer) As string 
>			Return Lands_GetLandByCubeInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_GetLandByPos_instance As Lazy(Of RemoteCallHandler_4(Of String,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandByPos"))
>		''' <summary> 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandByPos(x As Single,y As Single,z As Single,dimensionId As Integer) As string 
>			Return Lands_GetLandByPos_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_GetLandByPosInt_instance As Lazy(Of RemoteCallHandler_4(Of String,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandByPosInt"))
>		''' <summary> 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer) As string 
>			Return Lands_GetLandByPosInt_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_GetLandInfoByCube_instance As Lazy(Of RemoteCallHandler_7(Of String,Single,Single,Single,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByCube"))
>		''' <summary> 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandInfoByCube(x1 As Single,y1 As Single,z1 As Single,x2 As Single,y2 As Single,z2 As Single,dimensionId As Integer) As string 
>			Return Lands_GetLandInfoByCube_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_GetLandInfoByCubeInt_instance As Lazy(Of RemoteCallHandler_7(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByCubeInt"))
>		''' <summary> 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandInfoByCubeInt(x1 As Integer,y1 As Integer,z1 As Integer,x2 As Integer,y2 As Integer,z2 As Integer,dimensionId As Integer) As string 
>			Return Lands_GetLandInfoByCubeInt_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId)
>		End Function
>		Private Shared Lands_GetLandInfoByPos_instance As Lazy(Of RemoteCallHandler_4(Of String,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer)("PFLP", "Lands::GetLandInfoByPos"))
>		''' <summary> 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandInfoByPos(x As Single,y As Single,z As Single,dimensionId As Integer) As string 
>			Return Lands_GetLandInfoByPos_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_GetLandInfoByPosInt_instance As Lazy(Of RemoteCallHandler_4(Of String,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer)("PFLP", "Lands::GetLandInfoByPosInt"))
>		''' <summary> 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandInfoByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer) As string 
>			Return Lands_GetLandInfoByPosInt_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_SetLandInfoByPos_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Single,Single,Single,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::SetLandInfoByPos"))
>		''' <summary> 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>		Public Shared Function SetLandInfoByPos(x As Single,y As Single,z As Single,dimensionId As Integer,landinfo As String) As bool 
>			Return Lands_SetLandInfoByPos_instance.Value(x,y,z,dimensionId,landinfo)
>		End Function
>		Private Shared Lands_SetLandInfoByPosInt_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::SetLandInfoByPosInt"))
>		''' <summary> 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>		Public Shared Function SetLandInfoByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer,landinfo As String) As bool 
>			Return Lands_SetLandInfoByPosInt_instance.Value(x,y,z,dimensionId,landinfo)
>		End Function
>		Private Shared Lands_CreateLand2D_instance As Lazy(Of RemoteCallHandler_6(Of Boolean,Integer,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand2D"))
>		''' <summary> 新建领地 返回值类型：bool </summary>
>		Public Shared Function CreateLand2D(x1 As Integer,z1 As Integer,x2 As Integer,z2 As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CreateLand2D_instance.Value(x1,z1,x2,z2,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CreateLand3D_instance As Lazy(Of RemoteCallHandler_8(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CreateLand3D"))
>		''' <summary> 新建领地 返回值类型：bool </summary>
>		Public Shared Function CreateLand3D(x1 As Integer,y1 As Integer,z1 As Integer,x2 As Integer,y2 As Integer,z2 As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CreateLand3D_instance.Value(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_DeleteLandByPos_instance As Lazy(Of RemoteCallHandler_4(Of Boolean,Single,Single,Single,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer)("PFLP", "Lands::DeleteLandByPos"))
>		''' <summary> 删除指定坐标(float)的领地 返回值类型：bool </summary>
>		Public Shared Function DeleteLandByPos(x As Single,y As Single,z As Single,dimensionId As Integer) As bool 
>			Return Lands_DeleteLandByPos_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_DeleteLandByPosInt_instance As Lazy(Of RemoteCallHandler_4(Of Boolean,Integer,Integer,Integer,Integer))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer)("PFLP", "Lands::DeleteLandByPosInt"))
>		''' <summary> 删除指定坐标(int)的领地 返回值类型：bool </summary>
>		Public Shared Function DeleteLandByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer) As bool 
>			Return Lands_DeleteLandByPosInt_instance.Value(x,y,z,dimensionId)
>		End Function
>		Private Shared Lands_GetLandPermissionByPos_instance As Lazy(Of RemoteCallHandler_5(Of String,Single,Single,Single,Integer,String))(Function() RemoteCallAPI.ImportAs(Of String,Single,Single,Single,Integer,String)("PFLP", "Lands::GetLandPermissionByPos"))
>		''' <summary> 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandPermissionByPos(x As Single,y As Single,z As Single,dimensionId As Integer,playerXuid As String) As string 
>			Return Lands_GetLandPermissionByPos_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_GetLandPermissionByPosInt_instance As Lazy(Of RemoteCallHandler_5(Of String,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::GetLandPermissionByPosInt"))
>		''' <summary> 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>		Public Shared Function GetLandPermissionByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As string 
>			Return Lands_GetLandPermissionByPosInt_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckLandPermissionByPos_instance As Lazy(Of RemoteCallHandler_6(Of Boolean,String,Single,Single,Single,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,String,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckLandPermissionByPos"))
>		''' <summary> 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>		Public Shared Function CheckLandPermissionByPos(permissionId As String,x As Single,y As Single,z As Single,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckLandPermissionByPos_instance.Value(permissionId,x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckLandPermissionByPosInt_instance As Lazy(Of RemoteCallHandler_6(Of Boolean,String,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,String,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckLandPermissionByPosInt"))
>		''' <summary> 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>		Public Shared Function CheckLandPermissionByPosInt(permissionId As String,x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckLandPermissionByPosInt_instance.Value(permissionId,x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckPlayerIsLandOwnerByPos_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Single,Single,Single,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPos"))
>		''' <summary> 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool </summary>
>		Public Shared Function CheckPlayerIsLandOwnerByPos(x As Single,y As Single,z As Single,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckPlayerIsLandOwnerByPos_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckPlayerIsLandOwnerByPosInt_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt"))
>		''' <summary> 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool </summary>
>		Public Shared Function CheckPlayerIsLandOwnerByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckPlayerIsLandOwnerByPosInt_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckIsLandSharedToPlayerByPos_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Single,Single,Single,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Single,Single,Single,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPos"))
>		''' <summary> 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>		Public Shared Function CheckIsLandSharedToPlayerByPos(x As Single,y As Single,z As Single,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckIsLandSharedToPlayerByPos_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckIsLandSharedToPlayerByPosInt_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt"))
>		''' <summary> 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>		Public Shared Function CheckIsLandSharedToPlayerByPosInt(x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckIsLandSharedToPlayerByPosInt_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckPlayerHasCreateChestPermission_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasCreateChestPermission"))
>		''' <summary> 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>		Public Shared Function CheckPlayerHasCreateChestPermission(x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckPlayerHasCreateChestPermission_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>		Private Shared Lands_CheckPlayerHasOpenChestPermission_instance As Lazy(Of RemoteCallHandler_5(Of Boolean,Integer,Integer,Integer,Integer,String))(Function() RemoteCallAPI.ImportAs(Of Boolean,Integer,Integer,Integer,Integer,String)("PFLP", "Lands::CheckPlayerHasOpenChestPermission"))
>		''' <summary> 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>		Public Shared Function CheckPlayerHasOpenChestPermission(x As Integer,y As Integer,z As Integer,dimensionId As Integer,playerXuid As String) As bool 
>			Return Lands_CheckPlayerHasOpenChestPermission_instance.Value(x,y,z,dimensionId,playerXuid)
>		End Function
>	End Class
>	Public NotInheritable Class Money
>		Private Shared Money_Get_instance As Lazy(Of RemoteCallHandler_1(Of Long,String))(Function() RemoteCallAPI.ImportAs(Of Long,String)("PFLP", "Money::Get"))
>		''' <summary> 获取玩家(指定玩家名)金钱 返回值类型：long </summary>
>		Public Shared Function Get(playerXuid As String) As long 
>			Return Money_Get_instance.Value(playerXuid)
>		End Function
>		Private Shared Money_Add_instance As Lazy(Of RemoteCallHandler_void_3(Of String,Long,String))(Function() RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Add"))
>		''' <summary> 给玩家(指定玩家名)加钱 </summary>
>		Public Shared Sub Add(playerXuid As String,count As Long,info As String)  
>			Money_Add_instance.Value(playerXuid,count,info)
>		End Sub
>		Private Shared Money_Remove_instance As Lazy(Of RemoteCallHandler_void_3(Of String,Long,String))(Function() RemoteCallAPI.Import_As(Of String,Long,String)("PFLP", "Money::Remove"))
>		''' <summary> 给玩家(指定玩家名)减钱 </summary>
>		Public Shared Sub Remove(playerXuid As String,count As Long,info As String)  
>			Money_Remove_instance.Value(playerXuid,count,info)
>		End Sub
>	End Class
>End Module
> 
>```
></details>
>
>---
>
</details>


<details><summary><b>All Api in F# / F# 完整接口<b></summary>


>---
><details><summary>F# imports / 直接导入</summary>
>
>``` F#
>#r "LiteLoader.Net"
>open LiteLoader.RemoteCall
>
>// 设置全局配置文件（要求JSON字符串） 返回值类型：bool
>let General_SetConfig = RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig")
>// 获取全局配置文件（JSON字符串） 返回值类型：string
>let General_GetConfig = RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig")
>// 重新加载所有功能的配置文件
>let General_Reload = RemoteCallAPI.Import_As("PFLP", "General::Reload")
>// 设置命令禁用(可设置提示)
>let Command_SetCommandDisabled = RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled")
>// 设置命令启用
>let Command_SetCommandEnabled = RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled")
>// 翻译 返回值类型：string
>let Language_Translate = RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate")
>// 设置玩家昵称
>let ChatEx_SetNickName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName")
>// 设置玩家聊天时的名字
>let ChatEx_SetFakeName = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName")
>// 设置玩家聊天消息后缀
>let ChatEx_SetEnd = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd")
>// 设置玩家聊天消息前缀
>let ChatEx_SetStart = RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart")
>// 获取玩家昵称 返回值类型：string
>let ChatEx_GetNickName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName")
>// 获取玩家聊天时的名字 返回值类型：string
>let ChatEx_GetFakeName = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName")
>// 获取玩家聊天消息后缀 返回值类型：string
>let ChatEx_GetEnd = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd")
>// 获取玩家聊天消息前缀 返回值类型：string
>let ChatEx_GetStart = RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart")
>// 给指定方块描框
>let ParticlesGraphics_DrawBlock = RemoteCallAPI.Import_As<nativeint,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock")
>// 给指定区域描框
>let ParticlesGraphics_DrawBorder = RemoteCallAPI.Import_As<nativeint,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder")
>// 检查指定立方体区域(float)是否有领地 返回值类型：bool
>let Lands_CheckCubeHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand")
>// 检查指定立方体区域(int)是否有领地 返回值类型：bool
>let Lands_CheckCubeHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt")
>// 检查指定坐标(float)是否有领地 返回值类型：bool
>let Lands_CheckPosHasLand = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand")
>// 检查指定坐标(int)是否有领地 返回值类型：bool
>let Lands_CheckPosHasLandInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt")
>// 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube")
>// 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt")
>// 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos")
>// 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt")
>// 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByCube = RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube")
>// 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByCubeInt = RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt")
>// 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByPos = RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos")
>// 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string
>let Lands_GetLandInfoByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt")
>// 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>let Lands_SetLandInfoByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos")
>// 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool
>let Lands_SetLandInfoByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt")
>// 新建领地 返回值类型：bool
>let Lands_CreateLand2D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D")
>// 新建领地 返回值类型：bool
>let Lands_CreateLand3D = RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D")
>// 删除指定坐标(float)的领地 返回值类型：bool
>let Lands_DeleteLandByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos")
>// 删除指定坐标(int)的领地 返回值类型：bool
>let Lands_DeleteLandByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt")
>// 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>let Lands_GetLandPermissionByPos = RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos")
>// 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string
>let Lands_GetLandPermissionByPosInt = RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt")
>// 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>let Lands_CheckLandPermissionByPos = RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos")
>// 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool
>let Lands_CheckLandPermissionByPosInt = RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt")
>// 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool
>let Lands_CheckPlayerIsLandOwnerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos")
>// 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool
>let Lands_CheckPlayerIsLandOwnerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt")
>// 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>let Lands_CheckIsLandSharedToPlayerByPos = RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos")
>// 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool
>let Lands_CheckIsLandSharedToPlayerByPosInt = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt")
>// 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool
>let Lands_CheckPlayerHasCreateChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission")
>// 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool
>let Lands_CheckPlayerHasOpenChestPermission = RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission")
>// 获取玩家(指定玩家名)金钱 返回值类型：long
>let Money_Get = RemoteCallAPI.ImportAs<int64,string>("PFLP", "Money::Get")
>// 给玩家(指定玩家名)加钱
>let Money_Add = RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Add")
>// 给玩家(指定玩家名)减钱
>let Money_Remove = RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Remove")
>
>```
></details>
><details><summary>F# module / F# 模块类（推荐）</summary>
>
>``` F#
>#r "LiteLoader.Net"
>open LiteLoader.RemoteCall
>
>module public PFLP =
>  module public General =
>    let private General_SetConfig_instance = lazy RemoteCallAPI.ImportAs<bool,string>("PFLP", "General::SetConfig")
>    /// <summary> 设置全局配置文件（要求JSON字符串） 返回值类型：bool </summary>
>    let public SetConfig(jsonStr:string):bool =
>      General_SetConfig_instance.Value.Invoke(jsonStr)
>    let private General_GetConfig_instance = lazy RemoteCallAPI.ImportAs<string>("PFLP", "General::GetConfig")
>    /// <summary> 获取全局配置文件（JSON字符串） 返回值类型：string </summary>
>    let public GetConfig():string =
>      General_GetConfig_instance.Value.Invoke()
>    let private General_Reload_instance = lazy RemoteCallAPI.Import_As("PFLP", "General::Reload")
>    /// <summary> 重新加载所有功能的配置文件 </summary>
>    let public Reload():unit =
>      General_Reload_instance.Value.Invoke()
>  module public Command =
>    let private Command_SetCommandDisabled_instance = lazy RemoteCallAPI.Import_As<string,string,string>("PFLP", "Command::SetCommandDisabled")
>    /// <summary> 设置命令禁用(可设置提示) </summary>
>    let public SetCommandDisabled(playerXuid:string)(cmd:string)(feedback:string):unit =
>      Command_SetCommandDisabled_instance.Value.Invoke(playerXuid,cmd,feedback)
>    let private Command_SetCommandEnabled_instance = lazy RemoteCallAPI.Import_As<string,string>("PFLP", "Command::SetCommandEnabled")
>    /// <summary> 设置命令启用 </summary>
>    let public SetCommandEnabled(playerXuid:string)(cmd:string):unit =
>      Command_SetCommandEnabled_instance.Value.Invoke(playerXuid,cmd)
>  module public Language =
>    let private Language_Translate_instance = lazy RemoteCallAPI.ImportAs<string,string,string,string>("PFLP", "Language::Translate")
>    /// <summary> 翻译 返回值类型：string </summary>
>    let public Translate(fromLanguage:string)(toLanguage:string)(text:string):string =
>      Language_Translate_instance.Value.Invoke(fromLanguage,toLanguage,text)
>  module public ChatEx =
>    let private ChatEx_SetNickName_instance = lazy RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetNickName")
>    /// <summary> 设置玩家昵称 </summary>
>    let public SetNickName(playerXuid:string)(nickName:string):unit =
>      ChatEx_SetNickName_instance.Value.Invoke(playerXuid,nickName)
>    let private ChatEx_SetFakeName_instance = lazy RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetFakeName")
>    /// <summary> 设置玩家聊天时的名字 </summary>
>    let public SetFakeName(playerXuid:string)(fakeName:string):unit =
>      ChatEx_SetFakeName_instance.Value.Invoke(playerXuid,fakeName)
>    let private ChatEx_SetEnd_instance = lazy RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetEnd")
>    /// <summary> 设置玩家聊天消息后缀 </summary>
>    let public SetEnd(playerXuid:string)(endStr:string):unit =
>      ChatEx_SetEnd_instance.Value.Invoke(playerXuid,endStr)
>    let private ChatEx_SetStart_instance = lazy RemoteCallAPI.Import_As<string,string>("PFLP", "ChatEx::SetStart")
>    /// <summary> 设置玩家聊天消息前缀 </summary>
>    let public SetStart(playerXuid:string)(startStr:string):unit =
>      ChatEx_SetStart_instance.Value.Invoke(playerXuid,startStr)
>    let private ChatEx_GetNickName_instance = lazy RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetNickName")
>    /// <summary> 获取玩家昵称 返回值类型：string </summary>
>    let public GetNickName(playerXuid:string):string =
>      ChatEx_GetNickName_instance.Value.Invoke(playerXuid)
>    let private ChatEx_GetFakeName_instance = lazy RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetFakeName")
>    /// <summary> 获取玩家聊天时的名字 返回值类型：string </summary>
>    let public GetFakeName(playerXuid:string):string =
>      ChatEx_GetFakeName_instance.Value.Invoke(playerXuid)
>    let private ChatEx_GetEnd_instance = lazy RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetEnd")
>    /// <summary> 获取玩家聊天消息后缀 返回值类型：string </summary>
>    let public GetEnd(playerXuid:string):string =
>      ChatEx_GetEnd_instance.Value.Invoke(playerXuid)
>    let private ChatEx_GetStart_instance = lazy RemoteCallAPI.ImportAs<string,string>("PFLP", "ChatEx::GetStart")
>    /// <summary> 获取玩家聊天消息前缀 返回值类型：string </summary>
>    let public GetStart(playerXuid:string):string =
>      ChatEx_GetStart_instance.Value.Invoke(playerXuid)
>  module public ParticlesGraphics =
>    let private ParticlesGraphics_DrawBlock_instance = lazy RemoteCallAPI.Import_As<nativeint,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBlock")
>    /// <summary> 给指定方块描框 </summary>
>    let public DrawBlock(player:nativeint)(x:int)(y:int)(z:int)(r:float)(g:float)(b:float)(thickness:float)(time:float)(alpha:float):unit =
>      ParticlesGraphics_DrawBlock_instance.Value.Invoke(player,x,y,z,r,g,b,thickness,time,alpha)
>    let private ParticlesGraphics_DrawBorder_instance = lazy RemoteCallAPI.Import_As<nativeint,int,int,int,int,int,int,float,float,float,float,float,float>("PFLP", "ParticlesGraphics::DrawBorder")
>    /// <summary> 给指定区域描框 </summary>
>    let public DrawBorder(player:nativeint)(x1:int)(y1:int)(z1:int)(x2:int)(y2:int)(z2:int)(r:float)(g:float)(b:float)(thickness:float)(time:float)(alpha:float):unit =
>      ParticlesGraphics_DrawBorder_instance.Value.Invoke(player,x1,y1,z1,x2,y2,z2,r,g,b,thickness,time,alpha)
>  module public Lands =
>    let private Lands_CheckCubeHasLand_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,float,float,float,int>("PFLP", "Lands::CheckCubeHasLand")
>    /// <summary> 检查指定立方体区域(float)是否有领地 返回值类型：bool </summary>
>    let public CheckCubeHasLand(x1:float)(y1:float)(z1:float)(x2:float)(y2:float)(z2:float)(dimensionId:int):bool =
>      Lands_CheckCubeHasLand_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_CheckCubeHasLandInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int>("PFLP", "Lands::CheckCubeHasLandInt")
>    /// <summary> 检查指定立方体区域(int)是否有领地 返回值类型：bool </summary>
>    let public CheckCubeHasLandInt(x1:int)(y1:int)(z1:int)(x2:int)(y2:int)(z2:int)(dimensionId:int):bool =
>      Lands_CheckCubeHasLandInt_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_CheckPosHasLand_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::CheckPosHasLand")
>    /// <summary> 检查指定坐标(float)是否有领地 返回值类型：bool </summary>
>    let public CheckPosHasLand(x:float)(y:float)(z:float)(dimensionId:int):bool =
>      Lands_CheckPosHasLand_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_CheckPosHasLandInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::CheckPosHasLandInt")
>    /// <summary> 检查指定坐标(int)是否有领地 返回值类型：bool </summary>
>    let public CheckPosHasLandInt(x:int)(y:int)(z:int)(dimensionId:int):bool =
>      Lands_CheckPosHasLandInt_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_GetLandByCube_instance = lazy RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandByCube")
>    /// <summary> 获取立方体区域(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandByCube(x1:float)(y1:float)(z1:float)(x2:float)(y2:float)(z2:float)(dimensionId:int):string =
>      Lands_GetLandByCube_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_GetLandByCubeInt_instance = lazy RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandByCubeInt")
>    /// <summary> 获取立方体区域(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandByCubeInt(x1:int)(y1:int)(z1:int)(x2:int)(y2:int)(z2:int)(dimensionId:int):string =
>      Lands_GetLandByCubeInt_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_GetLandByPos_instance = lazy RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandByPos")
>    /// <summary> 获取指定坐标(float)领地信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandByPos(x:float)(y:float)(z:float)(dimensionId:int):string =
>      Lands_GetLandByPos_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_GetLandByPosInt_instance = lazy RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandByPosInt")
>    /// <summary> 获取指定坐标(int)领地信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandByPosInt(x:int)(y:int)(z:int)(dimensionId:int):string =
>      Lands_GetLandByPosInt_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_GetLandInfoByCube_instance = lazy RemoteCallAPI.ImportAs<string,float,float,float,float,float,float,int>("PFLP", "Lands::GetLandInfoByCube")
>    /// <summary> 获取立方体区域(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandInfoByCube(x1:float)(y1:float)(z1:float)(x2:float)(y2:float)(z2:float)(dimensionId:int):string =
>      Lands_GetLandInfoByCube_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_GetLandInfoByCubeInt_instance = lazy RemoteCallAPI.ImportAs<string,int,int,int,int,int,int,int>("PFLP", "Lands::GetLandInfoByCubeInt")
>    /// <summary> 获取立方体区域(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandInfoByCubeInt(x1:int)(y1:int)(z1:int)(x2:int)(y2:int)(z2:int)(dimensionId:int):string =
>      Lands_GetLandInfoByCubeInt_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId)
>    let private Lands_GetLandInfoByPos_instance = lazy RemoteCallAPI.ImportAs<string,float,float,float,int>("PFLP", "Lands::GetLandInfoByPos")
>    /// <summary> 获取指定坐标(float)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandInfoByPos(x:float)(y:float)(z:float)(dimensionId:int):string =
>      Lands_GetLandInfoByPos_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_GetLandInfoByPosInt_instance = lazy RemoteCallAPI.ImportAs<string,int,int,int,int>("PFLP", "Lands::GetLandInfoByPosInt")
>    /// <summary> 获取指定坐标(int)领地数据源详细信息（返回JSON字符串） 返回值类型：string </summary>
>    let public GetLandInfoByPosInt(x:int)(y:int)(z:int)(dimensionId:int):string =
>      Lands_GetLandInfoByPosInt_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_SetLandInfoByPos_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::SetLandInfoByPos")
>    /// <summary> 设置指定坐标(float)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>    let public SetLandInfoByPos(x:float)(y:float)(z:float)(dimensionId:int)(landinfo:string):bool =
>      Lands_SetLandInfoByPos_instance.Value.Invoke(x,y,z,dimensionId,landinfo)
>    let private Lands_SetLandInfoByPosInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::SetLandInfoByPosInt")
>    /// <summary> 设置或修改指定坐标(int)领地数据源详细信息（传入JSON字符串） 返回值类型：bool </summary>
>    let public SetLandInfoByPosInt(x:int)(y:int)(z:int)(dimensionId:int)(landinfo:string):bool =
>      Lands_SetLandInfoByPosInt_instance.Value.Invoke(x,y,z,dimensionId,landinfo)
>    let private Lands_CreateLand2D_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,int,string>("PFLP", "Lands::CreateLand2D")
>    /// <summary> 新建领地 返回值类型：bool </summary>
>    let public CreateLand2D(x1:int)(z1:int)(x2:int)(z2:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CreateLand2D_instance.Value.Invoke(x1,z1,x2,z2,dimensionId,playerXuid)
>    let private Lands_CreateLand3D_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,int,int,int,string>("PFLP", "Lands::CreateLand3D")
>    /// <summary> 新建领地 返回值类型：bool </summary>
>    let public CreateLand3D(x1:int)(y1:int)(z1:int)(x2:int)(y2:int)(z2:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CreateLand3D_instance.Value.Invoke(x1,y1,z1,x2,y2,z2,dimensionId,playerXuid)
>    let private Lands_DeleteLandByPos_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,int>("PFLP", "Lands::DeleteLandByPos")
>    /// <summary> 删除指定坐标(float)的领地 返回值类型：bool </summary>
>    let public DeleteLandByPos(x:float)(y:float)(z:float)(dimensionId:int):bool =
>      Lands_DeleteLandByPos_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_DeleteLandByPosInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int>("PFLP", "Lands::DeleteLandByPosInt")
>    /// <summary> 删除指定坐标(int)的领地 返回值类型：bool </summary>
>    let public DeleteLandByPosInt(x:int)(y:int)(z:int)(dimensionId:int):bool =
>      Lands_DeleteLandByPosInt_instance.Value.Invoke(x,y,z,dimensionId)
>    let private Lands_GetLandPermissionByPos_instance = lazy RemoteCallAPI.ImportAs<string,float,float,float,int,string>("PFLP", "Lands::GetLandPermissionByPos")
>    /// <summary> 获取指定坐标(float)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>    let public GetLandPermissionByPos(x:float)(y:float)(z:float)(dimensionId:int)(playerXuid:string):string =
>      Lands_GetLandPermissionByPos_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_GetLandPermissionByPosInt_instance = lazy RemoteCallAPI.ImportAs<string,int,int,int,int,string>("PFLP", "Lands::GetLandPermissionByPosInt")
>    /// <summary> 获取指定坐标(int)领地权限（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：string </summary>
>    let public GetLandPermissionByPosInt(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):string =
>      Lands_GetLandPermissionByPosInt_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckLandPermissionByPos_instance = lazy RemoteCallAPI.ImportAs<bool,string,float,float,float,int,string>("PFLP", "Lands::CheckLandPermissionByPos")
>    /// <summary> 检查指定坐标(float)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>    let public CheckLandPermissionByPos(permissionId:string)(x:float)(y:float)(z:float)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckLandPermissionByPos_instance.Value.Invoke(permissionId,x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckLandPermissionByPosInt_instance = lazy RemoteCallAPI.ImportAs<bool,string,int,int,int,int,string>("PFLP", "Lands::CheckLandPermissionByPosInt")
>    /// <summary> 检查指定坐标(int)领地是否有指定权限（permissionId参考GetLandPermissionByPos返回的key）（返回JSON字符串字典{key:boolean}）（可指定玩家否则playerXuid填写空字符串） 返回值类型：bool </summary>
>    let public CheckLandPermissionByPosInt(permissionId:string)(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckLandPermissionByPosInt_instance.Value.Invoke(permissionId,x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckPlayerIsLandOwnerByPos_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPos")
>    /// <summary> 检查玩家是否是指定坐标(float)领地的主人 返回值类型：bool </summary>
>    let public CheckPlayerIsLandOwnerByPos(x:float)(y:float)(z:float)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckPlayerIsLandOwnerByPos_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckPlayerIsLandOwnerByPosInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerIsLandOwnerByPosInt")
>    /// <summary> 检查玩家是否是指定坐标(int)领地的主人 返回值类型：bool </summary>
>    let public CheckPlayerIsLandOwnerByPosInt(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckPlayerIsLandOwnerByPosInt_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckIsLandSharedToPlayerByPos_instance = lazy RemoteCallAPI.ImportAs<bool,float,float,float,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPos")
>    /// <summary> 检查指定坐标(float)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>    let public CheckIsLandSharedToPlayerByPos(x:float)(y:float)(z:float)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckIsLandSharedToPlayerByPos_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckIsLandSharedToPlayerByPosInt_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckIsLandSharedToPlayerByPosInt")
>    /// <summary> 检查指定坐标(int)领地是否共享给指定玩家（检查具体权限请使用CheckLandPermissionByPos） 返回值类型：bool </summary>
>    let public CheckIsLandSharedToPlayerByPosInt(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckIsLandSharedToPlayerByPosInt_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckPlayerHasCreateChestPermission_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasCreateChestPermission")
>    /// <summary> 检查玩家在指定坐标(int)领地是否有开箱（方块交互）、放置、破坏的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>    let public CheckPlayerHasCreateChestPermission(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckPlayerHasCreateChestPermission_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>    let private Lands_CheckPlayerHasOpenChestPermission_instance = lazy RemoteCallAPI.ImportAs<bool,int,int,int,int,string>("PFLP", "Lands::CheckPlayerHasOpenChestPermission")
>    /// <summary> 检查玩家在指定坐标(int)领地是否有使用箱子的权限(主要用于锁箱插件) 返回值类型：bool </summary>
>    let public CheckPlayerHasOpenChestPermission(x:int)(y:int)(z:int)(dimensionId:int)(playerXuid:string):bool =
>      Lands_CheckPlayerHasOpenChestPermission_instance.Value.Invoke(x,y,z,dimensionId,playerXuid)
>  module public Money =
>    let private Money_Get_instance = lazy RemoteCallAPI.ImportAs<int64,string>("PFLP", "Money::Get")
>    /// <summary> 获取玩家(指定玩家名)金钱 返回值类型：long </summary>
>    let public Get(playerXuid:string):int64 =
>      Money_Get_instance.Value.Invoke(playerXuid)
>    let private Money_Add_instance = lazy RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Add")
>    /// <summary> 给玩家(指定玩家名)加钱 </summary>
>    let public Add(playerXuid:string)(count:int64)(info:string):unit =
>      Money_Add_instance.Value.Invoke(playerXuid,count,info)
>    let private Money_Remove_instance = lazy RemoteCallAPI.Import_As<string,int64,string>("PFLP", "Money::Remove")
>    /// <summary> 给玩家(指定玩家名)减钱 </summary>
>    let public Remove(playerXuid:string)(count:int64)(info:string):unit =
>      Money_Remove_instance.Value.Invoke(playerXuid,count,info)
>
>```
></details>
>
>---
>
</details>

