---
title: тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать обзор доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58abda6c89e484336b34d546edc68ebbfe432162
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579263"
---
# <a name="accessreviewreviewerscope-resource-type"></a>тип ресурса accessReviewReviewerScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это запрос OData, который позволяет рецензентам быть указанными как статический список пользователей (то есть конкретных пользователей, владельцев групп и членов группы) или динамически, в которых каждый пользователь просматривается их менеджером или владельцами групп. Чтобы создать самообзор (когда пользователи просматривают собственный доступ), не предоставлять рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Запрос, определяющий, кто будет рецензентом. Примеры см. в таблице. |
| queryType | Строка | Тип запроса. Примеры включают `MicrosoftGraph` и `ARM` . |
| queryRoot | Строка | В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство требуется только в том случае, если указан относительный запрос, `./manager` например. Возможное значение: `decisions` . |

Дополнительные возможности настройки для рецензентов см. в обзоре Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept)


## <a name="relationships"></a>Отношения
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
