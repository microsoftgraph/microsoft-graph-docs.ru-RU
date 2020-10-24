---
author: JeremyKelley
ms.date: 09/10/2017
title: Тип ресурса file
localization_priority: Normal
description: Ресурс File — это единая структура, объединяющая элементы данных, связанные с файлами.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c19f2afce6128c7fb29a81c6e8d8f2d1c08c7913
ms.sourcegitcommit: ab578b062c534db57844490f35e802df8a8f4dfa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2020
ms.locfileid: "48753397"
---
# <a name="file-resource-type"></a>Тип ресурса file

Пространство имен: microsoft.graph

Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.

Если [**DriveItem**](driveitem.md) имеет аспект **File** , отличный от NULL, элемент представляет файл.
Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.

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

