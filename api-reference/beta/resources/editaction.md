---
author: daspek
description: Наличие ресурса EditAction в ресурсе itemActivity указывает, что в результате выполнения действия элемент был изменен.
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 33d70965c945f2ad91d2ed9e609c1232284d7200
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089702"
---
# <a name="editaction-resource-type"></a>Тип ресурса EditAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **EditAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был изменен.

**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a>Свойства

Нет Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->


