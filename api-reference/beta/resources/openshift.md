---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3eff83475c4a36ec1c294c62b9e1b87673926d8d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895850"
---
# <a name="openshift-resource-type"></a>Тип ресурса Опеншифт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/openshift-get.md); | [опеншифт](openshift.md) | Чтение свойств и связей объекта Опеншифт. |
| [обновление](../api/openshift-update.md). | [опеншифт](openshift.md) | Обновление объекта Опеншифт. |
| [удаление](../api/openshift-delete.md); | Нет | Удаление объекта Опеншифт. |

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
