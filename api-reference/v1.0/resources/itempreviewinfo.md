---
author: kevinlam
title: Тип ресурса itemPreviewInfo
ms.localizationpriority: medium
description: Содержит сведения о том, как внедрить предварительную версию driveItem.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: d89f7ae60df58cb34891879fbc85c4e33cc9f8d7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899584"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса itemPreviewInfo

Пространство имен: microsoft.graph

Содержит сведения о том, как внедрить предварительную версию [driveItem](driveitem.md).

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
| getUrl         | string | URL-адрес, подходящий для внедрения с помощью HTTP GET (iframes и т. д.)
| postUrl        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (публикация формы, JS и т. д.)
| postParameters | string | Параметры POST, которые необходимо включить при использовании postUrl

В зависимости от текущего состояния поддержки указанных параметров может быть возвращено значение getUrl, postUrl или оба.

postParameters — `application/x-www-form-urlencoded`это строка в формате POST, и при выполнении postUrl-запроса тип контента должен быть задан соответствующим образом. Пример:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров должны считаться непрозрачными.

