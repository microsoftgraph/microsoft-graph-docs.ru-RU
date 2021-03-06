---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: Ресурс itemPreviewInfo содержит сведения о встраии предварительного просмотра ресурса driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240572"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса itemPreviewInfo

Пространство имен: microsoft.graph

Ресурс **itemPreviewInfo содержит** сведения о том, как встраить предварительный просмотр [ресурса driveItem.](driveitem.md)

## <a name="json-representation"></a>Представление JSON

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a>Свойства

| Имя           | Тип   | Описание
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т. д.)
| postUrl        | string | URL-адрес, подходящий для встраивки с помощью HTTP POST (публикация формы, JS и т. д.)
| postParameters | string | Параметры POST, которые необходимо включить при использовании postUrl

В зависимости от текущего состояния поддержки указанных параметров может быть возвращено либо getUrl, либо postUrl, либо оба этих параметра.

postParameters — это строка в формате , и если postUrl выполняет postUrl, тип контента `application/x-www-form-urlencoded` должен быть установлен соответствующим образом. Например,
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачной.

