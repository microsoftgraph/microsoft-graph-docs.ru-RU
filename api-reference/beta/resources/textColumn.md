---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: b57caa76f8376bbd7f119546009f3aca97b78385
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339834"
---
# <a name="textcolumn-resource-type"></a>Тип ресурса textColumn

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

| Имя свойства                   | Тип   | Описание
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | Указывает, разрешено ли отображать несколько строк текста.
| **appendChangesToExistingText** | string | Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.
| **linesForEditing**             | int    | Размер текстового поля.
| **maxLength**                   | int    | Максимальное количество символов для значения.
| **textType**                    | string | Тип хранимого текста. Должно иметь тип `plain` или `richText`

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
