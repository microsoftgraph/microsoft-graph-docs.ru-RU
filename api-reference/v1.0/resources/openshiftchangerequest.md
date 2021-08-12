---
title: тип ресурса openShiftChangeRequest
description: Представляет запрос на утверждение открытой смены в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a6f34e566caa2ff623eb3a66ebf8584b1adeb764dd1e7918bc34f1dbd8455a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229110"
---
# <a name="openshiftchangerequest-resource-type"></a>тип ресурса openShiftChangeRequest

Пространство имен: microsoft.graph

Представляет запрос на утверждение [openShift](../resources/openshift.md) в [расписании.](../resources/schedule.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/openshiftchangerequest-list.md) | Коллекция [openShiftChangeRequest](openshiftchangerequest.md) | Список свойств и связей **объектов openShiftChangeRequest** в группе. |
| [Создание](../api/openshiftchangerequest-post.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Создайте экземпляр **объекта openShiftChangeRequest.** |
| [Получение](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Ознакомьтесь с свойствами и отношениями объекта **openShiftChangeRequest.** |
|[Утвердить](../api/openshiftchangerequest-approve.md)|Нет|Утверждение запроса на изменение с открытой сменой.|
|[Отклонение](../api/openshiftchangerequest-decline.md)|Нет| Отклонение запроса на изменение с открытой сменой.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|openShiftId|String| ID для открытой смены.|

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

