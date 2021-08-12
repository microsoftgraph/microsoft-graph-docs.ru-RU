---
author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Тип ресурса Hashes
description: Ресурс хэшей группирует доступных хэши в единую структуру для элемента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd04ff57aff3d276655a173d123f228520a77b7d548afb9f8d75d30fd6ba4e6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243555"
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
| **sha1Hash**     | String | Хэш SHA1 для содержимого файла (если доступно). Только для чтения. |
| **sha256Hash**   | String | Хеш SHA256 для содержимого файла (при наличии). Только для чтения. |
| **crc32Hash**    | String | Значение CRC32 файла в маленьком endian (если доступно). Только для чтения.            |
| **quickXorHash** | Строка | Особый хэш файла, который можно использовать, чтобы определить, было ли изменено содержимое файла (если доступно). Только для чтения. |

**Примечание.** В некоторых случаях значения хэша могут быть недоступны. Если это так, значения хэша для определенного элемента будут обновлены после загрузки элемента.

## <a name="remarks"></a>Замечания

В OneDrive для бизнеса и SharePoint Server 2016 недоступны **sha1Hash** и **crc32Hash** и **sha256Hash.**

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

