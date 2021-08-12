---
author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9f8a5f333c0904732ef47bcac0c962f522d3ecd4c5e11a6884eaf396e354b49b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121307"
---
# <a name="choicecolumn-resource-type"></a>Тип ресурса choiceColumn

Пространство имен: microsoft.graph

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

| Имя свойства      | Тип               | Описание
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | boolean            | Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.
| **choices**        | Коллекция (string) | Список значений, доступных для данного столбца.
| **displayAs**      | string             | Способ отображения вариантов в пользовательском интерфейсе. Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->

