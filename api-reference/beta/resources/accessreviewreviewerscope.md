---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68f353b81b6a14292828d82929a0eeac81d67bc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469159"
---
# <a name="accessreviewreviewerscope-resource-type"></a>тип ресурса accessReviewReviewerScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это выражается как запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (например, конкретных пользователей, владельцев групп, членов группы) или динамически (т.е. в случае, когда каждый пользователь просматривается их менеджером). Чтобы создать самообзор (когда пользователи просматривают собственный доступ), не предоставлять рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | String | Запрос, определяющий, кто будет рецензентом. Примеры см. в таблице. |
| queryType | String | Тип запроса. Примеры включают `MicrosoftGraph` и `ARM` . |
| queryRoot | String | В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство требуется только в том случае, если указан относительный запрос (например, ./manager). |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Поддерживаемые запросы для accessReviewReviewerScope

|Сценарий| Запрос | queryType | queryRoot |
|--|--|--|--|
| Владелец группы в качестве рецензента | /groups/{group id}/owners |MicrosoftGraph||
| Конкретный пользователь в качестве рецензента | /users/{user id} |MicrosoftGraph||
| Менеджер пользователя, проверяемого в качестве рецензента | ./manager | MicrosoftGraph |решения|
| Самообсвятие | Пустой список (без рецензентов) | MicrosoftGraph  |


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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
