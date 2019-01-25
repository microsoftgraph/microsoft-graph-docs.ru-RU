---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: 551b09cee9fa662d357ee763b67ce78bea03425f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514847"
---
# <a name="hashes-resource-type"></a>Тип ресурса Hashes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **хэшей** группирует доступных хэши в единую структуру для элемента.

**Примечание.** Не все службы предоставляют значение для всех свойств хэша в списке.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип   | Описание                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Хэш SHA1 для содержимого файла (если доступно). Только для чтения. |
| **crc32Hash**    | String | Значение CRC32 файла (если доступно). Только для чтения.            |
| **quickXorHash** | Строка | Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения. |

**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.

## <a name="remarks"></a>Замечания

В OneDrive для бизнеса и SharePoint Server 2016 значения **sha1Hash** и **crc32Hash** недоступны.

В OneDrive персональный значение **quickXorHash** недоступно.

Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
