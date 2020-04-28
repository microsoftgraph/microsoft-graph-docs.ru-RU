---
author: daspek
description: Наличие ресурса CreateAction в ресурсе itemActivity указывает, что в результате выполнения действия был создан элемент.
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 349a46b4fc4b13fd597f120fdc4ca4d6641e932e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507368"
---
# <a name="createaction-resource-type"></a>Тип ресурса CreateAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Наличие ресурса **CreateAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия был создан элемент.

**Примечание.** На данный момент этот ресурс пуст, но в будущих редакциях API в него могут быть добавлены дополнительные свойства.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a>Свойства

Нет. Этот аспект принимает нулевое или ненулевое значение и не содержит свойств.

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
