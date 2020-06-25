---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Тип ресурса Hashes
description: Ресурс хэшей группирует доступных хэши в единую структуру для элемента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da326576b148fdaee79ebfc3df2d7832bfeee4e5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863742"
---
# <a name="hashes-resource-type"></a>Тип ресурса Hashes

Пространство имен: microsoft.graph

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
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>Свойства

| Свойство         | Тип   | Описание                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | SHA1 hash for the contents of the file (if available). Read-only. |
| **sha256Hash**   | String | Хэш SHA256 для содержимого файла (если он доступен). Только для чтения. |
| **crc32Hash**    | String | Значение CRC32 файла с прямым порядком байтов (при наличии). Только для чтения.            |
| **quickXorHash** | Строка | A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only. |

**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.

## <a name="remarks"></a>Замечания

В OneDrive для бизнеса и SharePoint Server 2016, **sha1Hash** и **Crc32Hash**, а **sha256Hash** недоступны.

В OneDrive персональный значение **quickXorHash** недоступно.

Сведения о том, как вычислить значение **quickXorHash** для файла, см. в [фрагменте кода QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).
Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
