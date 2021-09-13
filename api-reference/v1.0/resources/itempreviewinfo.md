---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.localizationpriority: medium
description: Ресурс itemPreviewInfo содержит сведения о том, как встраить предварительный просмотр driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e0a56b5129e67af8dc0ac7b360664eb31433d137
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084302"
---
# <a name="itempreviewinfo-resource-type"></a>тип ресурса itemPreviewInfo

Пространство имен: microsoft.graph

Ресурс **itemPreviewInfo содержит** сведения о том, как встраить предварительный просмотр [driveItem.](driveitem.md)

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
| getUrl         | string | URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т.д.)
| postUrl        | string | URL-адрес, подходящий для встраивки с помощью HTTP POST (столб формы, JS и т.д.)
| postParameters | string | Параметры POST, которые необходимо включить при использовании postUrl

Либо getUrl, postUrl, либо оба могут быть возвращены в зависимости от текущего состояния поддержки указанных параметров.

postParameters — это строка, отформатированная как, и при выполнении POST в postUrl тип контента должен быть задат `application/x-www-form-urlencoded` соответствующим образом. Примеры:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачной.

