---
title: Тип ресурса openShiftChangeRequest
description: Представляет тип запроса на смену для утверждения открытой смены в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161431"
---
# <a name="openshiftchangerequest-resource-type"></a>Тип ресурса openShiftChangeRequest

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип запроса на смену для утверждения [openshift](../resources/openshift.md) в [расписании.](../resources/schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/openshiftchangerequest-post.md) | [openshiftchangerequest](openshiftchangerequest.md) | Создание экземпляра объекта openshiftchangerequest. |
| [Список](../api/openshiftchangerequest-list.md) | Коллекция [openshiftchangerequest](openshiftchangerequest.md) | Список свойств и связей объектов **openShiftChangeRequest** в команде. |
| [Получение](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Чтение свойств и связей объекта **openShiftChangeRequest.** |
|[Утвердить](../api/openshiftchangerequest-approve.md)|Нет|Утверждение запроса на изменение открытой смены.|
|[Отклонение](../api/openshiftchangerequest-decline.md)|Нет| Отклонение запроса на изменение открытой смены.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|openShiftId|String| ИД для открытой смены.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
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


