---
author: JeremyKelley
description: Группы ресурсов хэширования, доступные в одной структуре для элемента.
ms.date: 09/10/2017
title: Hashes
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a4d6bf2851ded2de61ff48f30000e5b872c2c26e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899169"
---
# <a name="hashes-resource-type"></a>Тип ресурса hashes

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Группирует доступные хэши в одну структуру для элемента.

> [!NOTE]
> Не все службы предоставляют значение для всех перечисленных свойств хэша. В OneDrive для бизнеса и SharePoint Server 2016 **sha1Hash**, **crc32Hash** и **sha256Hash** недоступны. В OneDrive персональный хэш **quickXorHash** недоступен.

## <a name="properties"></a>Свойства

| Свойство         | Тип   | Описание                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | Хэш SHA1 для содержимого файла (если доступно). Только для чтения. |
| **sha256Hash**   | Строка | Хэш SHA256 для содержимого файла (если он доступен). Только для чтения. |
| **crc32Hash**    | String | Значение CRC32 файла (если доступно). Только для чтения.            |
| **quickXorHash** | Строка | Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения. |

> **Примечание:** В случаях, когда хэш-значения недоступны, хэш-значения элемента будут обновлены после скачивания элемента.

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


