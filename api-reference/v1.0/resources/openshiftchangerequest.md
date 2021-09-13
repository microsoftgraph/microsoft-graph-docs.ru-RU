---
title: тип ресурса openShiftChangeRequest
description: Представляет запрос на утверждение открытой смены в расписании.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ed6769b32a26625fe82a4fd51445ad71f8d213a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071982"
---
# <a name="openshiftchangerequest-resource-type"></a>тип ресурса openShiftChangeRequest

Пространство имен: microsoft.graph

Представляет запрос на утверждение [openShift](../resources/openshift.md) в [расписании.](../resources/schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/openshiftchangerequest-list.md) | Коллекция [openShiftChangeRequest](openshiftchangerequest.md) | Список свойств и связей **объектов openShiftChangeRequest** в группе. |
| [Создание](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Создайте экземпляр **объекта openShiftChangeRequest.** |
| [получение](../api/openshiftchangerequest-get.md); | [openShiftChangeRequest](openshiftchangerequest.md) | Ознакомьтесь с свойствами и отношениями объекта **openShiftChangeRequest.** |
|[Утвердить](../api/openshiftchangerequest-approve.md)|Нет|Утверждение запроса на изменение с открытой сменой.|
|[Отклонение](../api/openshiftchangerequest-decline.md)|Нет| Отклонение запроса на изменение с открытой сменой.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|openShiftId|Строка| ID для открытой смены.|

## <a name="relationships"></a>Отношения

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

