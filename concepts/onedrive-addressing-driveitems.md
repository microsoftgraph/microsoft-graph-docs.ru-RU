---
title: Обращение к ресурсам на диске в OneDrive
description: Узнайте о доступе к элементам на диске в OneDrive с помощью адресов на основе идентификаторов и путей, а также о правильном кодировании путей для Microsoft Graph.
ms.localizationpriority: high
ms.prod: sharepoint
author: JeremyKelley
doc_type: conceptualPageType
ms.openlocfilehash: 46f0304dc81245c79213f96cde30efb95766a580
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447123"
---
# <a name="address-resources-in-a-drive-on-onedrive"></a>Обращение к ресурсам на диске в OneDrive

Узнайте о доступе к элементам на диске в OneDrive с помощью адресов на основе идентификаторов и путей, а также о правильном кодировании путей для Microsoft Graph.

## <a name="id-based-addressing"></a>Обращение к элементам с использованием идентификаторов
OneDrive поддерживает обращение к элементам с использованием идентификаторов. При создании элементов им назначаются уникальные идентификаторы. Эти идентификаторы остаются неизменными при выполнении действий над элементами. При переименовании или перемещении элемента его идентификатор не изменяется.

Обращение к элементам с использованием идентификаторов — удобный способ отслеживания элементов, которые пользователь может перемещать в различные расположения в OneDrive. Если у вас есть идентификатор существующего элемента, вы сможете найти этот элемент.

## <a name="path-based-addressing"></a>Обращение к элементам с использованием пути
OneDrive также поддерживает обращение к элементам с использованием пути. Такой способ позволяет использовать понятный синтаксис URL-адресов для обращения к элементам относительно иерархии элементов, видимой в OneDrive. Если вы знаете иерархию, ведущую к элементу, вы можете напрямую обратиться к нему, не тратя время на выполнение повторяющихся вызовов для обнаружения каждого уровня иерархии.

Так как при обращении к элементу с использованием пути применяется имя элемента, при переименовании элемента или перемещении его в другое расположение путь к элементу изменится.

Вы можете использовать адресацию на основе путей относительно любого элемента в OneDrive. Например, при работе с общими папками вы можете использовать URL-адрес на основе пути, относительный для идентификатора элемента общей папки, для обращения к каким-либо объектам в общей папке с использованием пути.

## <a name="examples"></a>Примеры
В следующих примерах показаны различные форматы URL-адресов для доступа к данным.
Все эти URL-адреса логически эквивалентны и возвращают содержимое файла MyFile.xlsx.

| Пример URL-адреса                                       | Описание                                              |
|:--------------------------------------------------|:---------------------------------------------------------|
| `/drive/root:/Documents/MyFile.xlsx:/content`     | Указан с использованием пути, относительного для корня диска.       |
| `/drive/special/documents:/MyFile.xlsx:/content`  | Указан с использованием имени файла в специальной папке `documents`. |
| `/drive/items/0123456789AB/content`               | Указан с использованием идентификатора элемента.                                    |
| `/drives/AB0987654321/items/0123456789AB/content` | Указан с использованием идентификатора диска и идентификатора элемента.                       |


## <a name="path-encoding"></a>Кодировка символов пути

OneDrive поддерживает обращение к файлам и папкам с использованием пути к элементу в OneDrive пользователя. Так как путь содержит указанный пользователем контент, который может содержать символы, небезопасные для использования в URL-адресе, вы должны проверить правильность кодировки всех сегментов пути.

При работе с Microsoft Graph предполагается, что URL-адреса соответствуют требованиям документа [RFC 3986](http://tools.ietf.org/html/rfc3986). Ниже кратко описано, как правильно кодировать пути для Microsoft Graph.

### <a name="onedrive-reserved-characters"></a>Символы, зарезервированные в OneDrive
Указанные ниже символы зарезервированы в OneDrive. Их не следует использовать в именах папок и файлов в OneDrive.

```
  onedrive-reserved  = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|"
  onedrive-business-reserved
                     = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|" / "#" / "%"
```

> [!NOTE]
> - Имена папок не должны оканчиваться точкой (`.`).
> - Имена файлов и папок не должны начинаться с тильды (~).
>
> Дополнительные сведения см. в разделе [Ограничения при синхронизации библиотек SharePoint с компьютером с помощью OneDrive для работы или учебы](https://support.microsoft.com/en-us/kb/2933738).

### <a name="uri-path-characters"></a>Символы, используемые в пути URI

При создании сегмента пути URL-адреса для API Microsoft Graph в именах путей, основанных на RFC URI, можно использовать указанные ниже символы.

```
  pchar       = unreserved / pct-encoded / sub-delims / ":" / "@"
  pct-encoded = "%" HEXDIG HEXDIG
  unreserved  = ALPHA / DIGIT / "-" / "." / "_" / "~"
  sub-delims  = "!" / "$" / "&" / "'" / "(" / ")"
              / "*" / "+" / "," / ";" / "="
```

Для символов в именах элементов, не включенных в группу `pchar`, например `#` и ` ` (пробел), необходимо применять кодировку с использованием символа процента.

### <a name="encoding-characters"></a>Кодирование символов
В Microsoft Graph применяется стандартная кодировка с использованием символа процента, в которой символы, недопустимые в URL-адресах, кодируются с использованием символа %, за которым следует код символа в таблице символов UTF-8. Пример:

* `" "` -> `%20`
* `"#"` -> `%23`

### <a name="common-url-encoding-mistakes"></a>Распространенные ошибки при кодировании URL-адресов
Вам не удастся закодировать весь URL-адрес с использованием одного вызова, так как для каждого сегмента URL-адреса используются различные правила кодирования. Если закодировать URL-адрес неправильно, не всегда будет понятно, в каком сегменте находится то или иное содержимое. Таким образом, при создании строки URL-адреса вам необходимо закодировать путь URL-адреса.

Например, вместо этого:

```
string url = url_encode("https://graph.microsoft.com/v1.0/me/drive/root:/" + path + ":/children")
```

Напишите это:

```
string url = "https://graph.microsoft.com/v1.0/me/drive/root:/" + url_path_encode(path) + ":/children")
```

Не во всех библиотеках кодирования URL-адресов соблюдаются все требования стандартного кодирования путей URL-адресов.

### <a name="net--c-sharp--visual-basic"></a>.NET, C-Sharp и Visual Basic

Классы .NET для `HttpUtility` и `Uri` включают различные методы кодирования URL-адресов. Тем не менее ни один из этих методов не может правильно кодировать все зарезервированные символы для компонента пути URL-адреса (включая `HttpUtility.UrlPathEncode`).

Вместо этих методов для создания правильного URL-адреса используйте `UriBuilder`.

```csharp
UriBuilder builder = new UriBuilder("https://graph.microsoft.com");
builder.Path = "/v1.0/me/drive/root:/Documents/My Files/#nine.docx";
Uri url = builder.Uri;
```

### <a name="objective-c--ios"></a>Objective-C и iOS

При разработке для Objective-C, iOS и Mac OS X для правильного кодирования компонента пути URL-адреса используйте метод `stringByAddingPercentEncodingWithAllowedCharacters` и `[NSCharacterSet URLPathAllowedCharacterSet]`.

```objc
NSString *root = @"https://graph.microsoft.com/v1.0/me/drive/root:/";
NSString *path = @"Documents/My Files/#nine.docx";
NSString *encPath = [path stringByAddingPercentEncodingWithAllowedCharacters:[NSCharacterSet URLPathAllowedCharacterSet]];
NSURL *url = [[NSURL alloc] initWithString:[root stringByAppendingString:encPath]];
```


### <a name="android"></a>Android

Для создания правильно закодированного URL-адреса используйте класс `Uri.Builder`.

```java
Uri.Builder builder = new Uri.Builder();
builder.
  scheme("https").
  authority("graph.microsoft.com").
  appendPath("v1.0").
  appendPath("me").
  appendPath("drive").
  appendPath("root:").
  appendPath("Documents").
  appendPath("My Files").
  appendPath("#nine.docx");
String url = builder.build().toString();
```

### <a name="javascript"></a>JavaScript

Для правильного кодирования компонента пути в JavaScript используйте `escape()`.

```javascript
var root = "https://graph.microsoft.com/v1.0/me/drive/root:";
var path = "/Documents/My Files/#nine.docx";
var url = root + escape(path);
```

### <a name="examples"></a>Примеры

Вот пример пользователя OneDrive (Adele) с указанной ниже иерархией папок.
```
OneDrive
    \Adele's Files
        \doc (1).docx
    \estimate%s.docx
    \Break#Out
        \saved_game[1].bin
```

Для обращения к любым файлам пользователя Adele необходимо применять кодирование с использованием знака процента, как показано ниже.

| Путь                     | Закодированный URL-адрес для пути                      |
|:-------------------------|:------------------------------------------|
| `\Adele's Files`          | `/root:/Adele's%20Files`                   |
| `\...\doc (1).docx`      | `/root:/Adele's%20Files/doc%20(1).docx`    |
| `\...\estimate%.docx`    | `/root:/Adele's%20Files/estimate%25s.docx` |
| `\Break#Out`             | `/root:/Break%23Out`                      |
| `\...\saved_game[1].bin` | `/root:/Break%23Out/saved_game[1].bin`    |

## <a name="see-also"></a>См. также

- [Обзор API для хранилища файлов OneDrive](onedrive-concept-overview.md)