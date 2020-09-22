---
title: Тип ресурса Опеншифтчанжерекуест
description: Представляет тип запроса на сдвиг для утверждения открытого сдвига в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 26dccf0d0e79e2f0427f07035ee31e5480c52b95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998560"
---
# <a name="openshiftchangerequest-resource-type"></a>Тип ресурса Опеншифтчанжерекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для утверждения [опеншифт](../resources/openshift.md) по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/openshiftchangerequest-post.md) | [опеншифтчанжерекуест](openshiftchangerequest.md) | Создайте экземпляр объекта опеншифтчанжерекуест. |
| [List](../api/openshiftchangerequest-list.md) | Коллекция [опеншифтчанжерекуест](openshiftchangerequest.md) | Перечисление свойств и связей объектов **опеншифтчанжерекуест** в команде. |
| [получение](../api/openshiftchangerequest-get.md); | [опеншифтчанжерекуест](openshiftchangerequest.md) | Чтение свойств и связей объекта **опеншифтчанжерекуест** . |
|[Утвердить](../api/openshiftchangerequest-approve.md)|Нет|Утверждение запроса на изменение открытого сочетания клавиш.|
|[Отклоня](../api/openshiftchangerequest-decline.md)|Нет| Отклонить запрос на изменение открытого Shift.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|опеншифтид|String| Идентификатор для открытой смены.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


