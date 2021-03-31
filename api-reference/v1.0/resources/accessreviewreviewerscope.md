---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469675"
---
# <a name="accessreviewreviewerscope-resource-type"></a>тип ресурса accessReviewReviewerScope

Пространство имен: microsoft.graph

AccessReviewReviewerScope определяет, кто указан в [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) для просмотра [appConsentRequests](../resources/appconsentrequest.md) и [userConsentRequests](../resources/appconsentrequest.md). Это выражается как запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (например, конкретных пользователей, владельцев групп, членов группы) или динамически (т.е. в случае, когда каждый пользователь просматривается их менеджером).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Запрос|String|Запрос, определяющий, кто будет рецензентом. Примеры см. в таблице. |
|queryRoot|String|Тип запроса. Примеры включают `MicrosoftGraph` и `ARM` .|
|queryType|String|В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство требуется только в том случае, если указан относительный запрос (например, `./manager` ).|

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Поддерживаемые запросы для accessReviewReviewerScope

|Сценарий| Запрос | queryType | queryRoot |
|--|--|--|--|
| Владелец группы в качестве рецензента | /groups/{group id}/owners |MicrosoftGraph||
| Конкретный пользователь в качестве рецензента | /users/{user id} |MicrosoftGraph||
| Менеджер пользователя, проверяемого в качестве рецензента | ./manager | MicrosoftGraph |решения|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
