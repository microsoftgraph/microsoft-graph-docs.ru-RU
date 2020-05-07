---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2051dddb78121341d22dc9e3cd20b13178cb81c9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154993"
---
# <a name="openshift-resource-type"></a>Тип ресурса Опеншифт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List](../api/openshift-list.md) | Коллекция [опеншифт](openshift.md) | Перечисление свойств и связей объектов **опеншифт** в команде.|
| [создание](../api/openshift-post.md); | [опеншифт](openshift.md) | Создайте экземпляр объекта **опеншифт** . |
| [получение](../api/openshift-get.md); | [опеншифт](openshift.md) | Чтение свойств и связей объекта **опеншифт** . |
| [обновление](../api/openshift-update.md). | [опеншифт](openshift.md) | Обновление объекта **опеншифт** . |
| [удаление](../api/openshift-delete.md); | Нет | Удаление объекта **опеншифт** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|драфтопеншифт|[опеншифтитем](openshiftitem.md)|Неопубликованная открытая смена.|
|schedulingGroupId|Строка|Идентификатор группы планирования, к которой относится открытая смена.|
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
