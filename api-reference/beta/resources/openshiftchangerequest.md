---
title: Тип ресурса Опеншифтчанжерекуест
description: Представляет тип запроса на сдвиг для утверждения открытого сдвига в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 400444ccccc13d103420cc95c522a6ed0aa1afa6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895849"
---
# <a name="openshiftchangerequest-resource-type"></a>Тип ресурса Опеншифтчанжерекуест

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на сдвиг для утверждения [опеншифт](../resources/openshift.md) по [расписанию](../resources/schedule.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/openshiftchangerequest-get.md); | [опеншифтчанжерекуест](openshiftchangerequest.md) | Чтение свойств и связей объекта **опеншифтчанжерекуест** . |
| [обновление](../api/openshiftchangerequest-update.md). | [опеншифтчанжерекуест](openshiftchangerequest.md) | Обновление объекта **опеншифтчанжерекуест** . |
| [удаление](../api/openshiftchangerequest-delete.md); | Нет | Удаление объекта **опеншифтчанжерекуест** . |
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
