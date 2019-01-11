---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: textColumn
localization_priority: Normal
ms.openlocfilehash: d064253cfad141d5879afb52451ca28fa2aeca67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860881"
---
# <a name="textcolumn-resource-type"></a>Тип ресурса textColumn

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
