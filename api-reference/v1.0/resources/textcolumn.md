---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 62711f2f44004e5b3d594eb472b7c018205d9e31
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239276"
---
# <a name="textcolumn-resource-type"></a>Тип ресурса textColumn

Пространство имен: microsoft.graph

Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **textColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a>Свойства

| Имя свойства                   | Тип    | Описание
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | boolean | Указывает, разрешено ли отображать несколько строк текста.
| **appendChangesToExistingText** | boolean | Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.
| **linesForEditing**             | int32   | Размер текстового поля.
| **maxLength**                   | int32   | Максимальное количество символов для значения.
| **textType**                    | string  | Тип хранимого текста. Должно иметь тип `plain` или `richText`

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->

