---
author: kevinlam
description: Ресурс ItemPreviewInfo содержит сведения о том, как внедрить предварительную версию DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo — OneDrive API
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 49c792845205b8b42b70961185da4ca46bee2fb7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176971"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса ItemPreviewInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **ItemPreviewInfo** содержит сведения о том, как внедрить предварительную версию [DriveItem](driveitem.md).

## <a name="json-representation"></a>Представление JSON

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                                      |
| :------------- | :----- | :--------------------------------------------------------------- |
| getUrl         | string | URL-адрес, подходящий для внедрения с помощью HTTP GET (iframes и т. д.)        |
| postUrl        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (публикация формы, JS и т. д.) |
| postParameters | string | Параметры POST, которые необходимо включить при использовании postUrl                      |

В зависимости от текущего состояния поддержки указанных параметров может быть возвращено значение getUrl, postUrl или оба.

postParameters — `application/x-www-form-urlencoded`это строка в формате POST, и при выполнении postUrl-запроса тип контента должен быть задан соответствующим образом. Например:

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров должны считаться непрозрачными.
