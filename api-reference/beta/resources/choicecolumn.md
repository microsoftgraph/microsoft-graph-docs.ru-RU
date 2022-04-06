---
author: JeremyKelley
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.date: 09/11/2017
title: choiceColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d7c2e1292bc3868b188b9389a0c44477606cbb3e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722257"
---
# <a name="choicecolumn-resource-type"></a>Тип ресурса choiceColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **choiceColumn** в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>Свойства

| Свойство           | Тип               | Описание                                                                                                   |
| :----------------- | :----------------- | :------------------------------------------------------------------------------------------------------------ |
| **allowTextEntry** | boolean            | Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.                                          |
| **choices**        | Коллекция (string) | Список значений, доступных для данного столбца.                                                                 |
| **displayAs**      | string             | Способ отображения вариантов в пользовательском интерфейсе. Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
