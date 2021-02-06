---
title: Тип ресурса accessReviewReviewerScope
description: Представляет, кто будет рассматривать проверку доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133492"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Тип ресурса accessReviewReviewerScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

AccessReviewReviewerScope определяет, кто будет рассматривать экземпляры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это выражается в виде запроса OData, который позволяет рецензентам быть задан как статический список пользователей (т. е. определенных пользователей, владельцев групп, членов группы) или динамически (т. е. в случае, когда каждый пользователь просматривается руководителем). Чтобы создать самообзор (когда пользователи проверяют собственный доступ), не выдавайте рецензентов при создании [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)


## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Запрос, определяющий, кто будет рецензентом. Примеры см. в таблице. |
| queryType | Строка | Тип запроса. Примеры: `MicrosoftGraph` и `ARM` . |
| queryRoot | Строка | В сценарии, где проверяющих необходимо указать динамически, это свойство используется для указать относительный источник запроса. Это свойство необходимо, только если указан относительный запрос (например, ./manager). |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Поддерживаемые запросы для accessReviewReviewerScope

|Сценарий| Запрос | queryType | queryRoot |
|--|--|--|--|
| Владелец группы в качестве рецензента | /groups/{group id}/owners |MicrosoftGraph||
| Конкретный пользователь в качестве рецензента | /users/{user id} |MicrosoftGraph||
| Руководитель пользователя, проверяемого в качестве рецензента | ./manager | MicrosoftGraph |decisions|

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
