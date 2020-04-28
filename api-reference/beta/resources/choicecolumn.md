---
author: JeremyKelley
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8b9b6db64bb1215a4be3fde10bce1a40bb5ffce3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507686"
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

| Имя свойства      | Тип               | Описание
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | boolean            | Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.
| **choices**        | Коллекция (string) | Список значений, доступных для данного столбца.
| **displayAs**      | string             | Способ отображения вариантов в пользовательском интерфейсе. Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.


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
