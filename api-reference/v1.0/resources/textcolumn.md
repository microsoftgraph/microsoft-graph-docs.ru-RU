---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 26d03141bc0520d4d957e853af28c241771d8dac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084008"
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

