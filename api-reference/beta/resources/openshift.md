---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f3ce94c12328e9c05f899c5d2176339bbed93432
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951939"
---
# <a name="openshift-resource-type"></a>Тип ресурса Опеншифт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/openshift-post.md) | [опеншифт](openshift.md) | Создайте экземпляр объекта **опеншифт** . |
| [List](../api/openshift-list.md) | Коллекция [опеншифт](openshift.md) | Перечисление свойств и связей объектов **опеншифт** в команде.|
| [получение](../api/openshift-get.md); | [опеншифт](openshift.md) | Чтение свойств и связей объекта **опеншифт** . |
| [обновление](../api/openshift-update.md). | [опеншифт](openshift.md) | Обновление объекта **опеншифт** . |
| [Удаление](../api/openshift-delete.md) | Нет | Удаление объекта **опеншифт** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|драфтопеншифт|[опеншифтитем](openshiftitem.md)|Неопубликованная открытая смена.|
|schedulingGroupId|String|Идентификатор группы планирования, к которой относится открытая смена.|
|шаредопеншифт|[опеншифтитем](openshiftitem.md)|Опубликованная открытая смена.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
