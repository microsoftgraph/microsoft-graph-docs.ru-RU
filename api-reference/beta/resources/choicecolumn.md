---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074826"
---
# <a name="choicecolumn-resource-type"></a>Тип ресурса choiceColumn

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| **allowTextEntry** | логический            | Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.
| **choices**        | Коллекция (string) | Список значений, доступных для данного столбца.
| **displayAs**      | строка             | Способ отображения вариантов в пользовательском интерфейсе. Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
