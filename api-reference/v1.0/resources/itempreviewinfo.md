---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: Ресурс itemPreviewInfo содержит сведения о том, как встраить предварительный просмотр driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d6a3eaac24991c4c95da0dd4b4ae2640d6462f95c25b47d0fcbea6ff459962ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130053"
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
| getUrl         | Строка | URL-адрес, подходящий для встраивки с помощью HTTP GET (iframes и т.д.)
| postUrl        | Строка | URL-адрес, подходящий для встраивки с помощью HTTP POST (столб формы, JS и т.д.)
| postParameters | Строка | Параметры POST, которые необходимо включить при использовании postUrl

Либо getUrl, postUrl, либо оба могут быть возвращены в зависимости от текущего состояния поддержки указанных параметров.

postParameters — это строка, отформатированная как, и при выполнении POST в postUrl тип контента должен быть задат `application/x-www-form-urlencoded` соответствующим образом. Например,
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачной.

