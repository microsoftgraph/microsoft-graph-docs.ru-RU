---
author: JeremyKelley
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8a6e8d3a06c3d34a321ec2fb5ff5d83586accb56
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724289"
---
# <a name="textcolumn-resource-type"></a>Тип ресурса textColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Свойство                        | Тип   | Описание                                                                   |
| :------------------------------ | :----- | :---------------------------------------------------------------------------- |
| **allowMultipleLines**          | string | Указывает, разрешено ли отображать несколько строк текста.                                      |
| **appendChangesToExistingText** | string | Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его. |
| **linesForEditing**             | int    | Размер текстового поля.                                                     |
| **maxLength**                   | int    | Максимальное количество символов для значения.                               |
| **textType**                    | string | Тип хранимого текста. Должно иметь тип `plain` или `richText`           |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
