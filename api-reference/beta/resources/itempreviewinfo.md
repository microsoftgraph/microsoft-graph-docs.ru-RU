---
author: kevinlam
description: Ресурс ItemPreviewInfo содержит сведения о том, как встраить предварительный просмотр DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo — OneDrive API
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9e4f3b390fe21284791b6c40d19d4de71ec3548b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723348"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса ItemPreviewInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **ItemPreviewInfo содержит** сведения о том, как встраить предварительный просмотр [DriveItem](driveitem.md).

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
| getUrl         | строка | URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т.д.)        |
| postUrl        | string | URL-адрес, подходящий для встраивки с помощью HTTP POST (столб формы, JS и т.д.) |
| postParameters | string | Параметры POST, которые необходимо включить при использовании postUrl                      |

Либо getUrl, postUrl, либо оба могут быть возвращены в зависимости от текущего состояния поддержки указанных параметров.

postParameters `application/x-www-form-urlencoded`— это строка, отформатированная как, и при выполнении POST в postUrl тип контента должен быть задат соответствующим образом. Например:

```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачной.
