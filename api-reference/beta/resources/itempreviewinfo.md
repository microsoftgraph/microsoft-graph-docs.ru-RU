---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: 'Итемпревиевинфо: API OneDrive'
localization_priority: Normal
ms.openlocfilehash: 469679e9baa016560f5a02425bc41d628a24dc2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562869"
---
# <a name="itempreviewinfo-resource-type"></a>Тип ресурса Итемпревиевинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **итемпревиевинфо** содержит сведения о внедрении предварительного просмотра [DriveItem](driveitem.md).

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
| Команда         | string | URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)
| Постурл        | string | URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)
| Параметры | string | Параметры POST для включения при использовании Постурл

В зависимости от текущего состояния поддержки для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.

i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры. Примеры:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

Форматы URL-адресов и параметров следует считать непрозрачными.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/itempreviewinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
