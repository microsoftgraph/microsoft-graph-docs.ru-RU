---
author: JeremyKelley
description: Хеш-коды групп ресурсов, доступные в виде одной структуры для элемента.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: df3629be679b714805ea6618b7aa963214f32793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013610"
---
# <a name="hashes-resource-type"></a>Тип ресурса hashs

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Группирует доступные хэши в единую структуру для элемента.

> [!NOTE]
> Не все службы предоставляют значение для всех перечисленных свойств хеша. В OneDrive для бизнеса и SharePoint Server 2016, **sha1Hash**, **crc32Hash**и **sha256Hash** недоступны. В OneDrive персональный хэш **quickXorHash** недоступен.

## <a name="properties"></a>Свойства

| Свойство         | Тип   | Описание                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Хэш SHA1 для содержимого файла (если доступно). Только для чтения. |
| **sha256Hash**   | String | Хэш SHA256 для содержимого файла (если он доступен). Только для чтения. |
| **crc32Hash**    | String | Значение CRC32 файла (если доступно). Только для чтения.            |
| **quickXorHash** | Строка | Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения. |

> **Примечание:** В случаях, когда хэш-значения недоступны, значения хеша для элемента будут обновлены после загрузки элемента.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="see-also"></a>См. также

- Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).
- Пример вычисления значения **quickXorHash** для файла см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->


