---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c551ce7568cb31f92d2bf02bb328ffa77fa95d63c8aca547b2add5e5cb57469
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211815"
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
| **allowMultipleLines**          | логический | Указывает, разрешено ли отображать несколько строк текста.
| **appendChangesToExistingText** | логический | Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.
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

