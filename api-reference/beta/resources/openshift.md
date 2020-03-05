---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e544f54c7fbf015ed1050ab23d76217b311bdeaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522195"
---
# <a name="openshift-resource-type"></a>Тип ресурса Опеншифт

Пространство имен: Microsoft. Graph

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
