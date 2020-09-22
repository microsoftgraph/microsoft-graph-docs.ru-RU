---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 534756fd26fcac13d150e9cbd1782a8f334e5a2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998567"
---
# <a name="openshift-resource-type"></a>Тип ресурса Опеншифт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/openshift-post.md) | [опеншифт](openshift.md) | Создайте экземпляр объекта **опеншифт** . |
| [List](../api/openshift-list.md) | Коллекция [опеншифт](openshift.md) | Перечисление свойств и связей объектов **опеншифт** в команде.|
| [получение](../api/openshift-get.md); | [опеншифт](openshift.md) | Чтение свойств и связей объекта **опеншифт** . |
| [обновление](../api/openshift-update.md). | [опеншифт](openshift.md) | Обновление объекта **опеншифт** . |
| [удаление](../api/openshift-delete.md); | Нет | Удаление объекта **опеншифт** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|драфтопеншифт|[опеншифтитем](openshiftitem.md)|Неопубликованная открытая смена.|
|schedulingGroupId|String|Идентификатор группы планирования, к которой относится открытая смена.|
|шаредопеншифт|[опеншифтитем](openshiftitem.md)|Опубликованная открытая смена.|

## <a name="relationships"></a>Связи

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


