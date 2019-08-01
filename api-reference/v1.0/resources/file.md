---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Файл
localization_priority: Normal
description: Ресурс File — это единая структура, объединяющая элементы данных, связанные с файлами.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 51ec91a635db2ca259ba84cea29304e4e6ac7cbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030375"
---
# <a name="file-resource-type"></a>Тип ресурса file

Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.

Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип                    | Описание                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| hashes   | [Hashes](hashes.md) | Хэши двоичного содержимого файла (если они доступны). Только для чтения.                                                                                    |
| mimeType | string                  | Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения. |

## <a name="remarks"></a>Замечания 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
