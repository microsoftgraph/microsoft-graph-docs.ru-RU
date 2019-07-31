---
author: JeremyKelley
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964344"
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
