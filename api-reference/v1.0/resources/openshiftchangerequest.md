---
title: Тип ресурса openShiftChangeRequest
description: Представляет запрос на утверждение открытой смены в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b427d7914d95aaed794734bbbb39fa3eb139d06a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158683"
---
# <a name="openshiftchangerequest-resource-type"></a>Тип ресурса openShiftChangeRequest

Пространство имен: microsoft.graph

Представляет запрос на утверждение [openShift](../resources/openshift.md) в [расписании.](../resources/schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/openshiftchangerequest-list.md) | Коллекция [openShiftChangeRequest](openshiftchangerequest.md) | Список свойств и связей объектов **openShiftChangeRequest** в команде. |
| [Создание](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Создание экземпляра объекта **openShiftChangeRequest.** |
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

