---
title: Тип ресурса accessReviewReviewerScope
description: Представляет, кто будет проверять проверку доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fbbb8288216eda745acc831c7b362454dfaec239
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698095"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Тип ресурса accessReviewReviewerScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

AccessReviewReviewerScope определяет, кто будет проверять экземпляры [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Это запрос OData, который позволяет рецензентам указать как статический список пользователей (то есть конкретных пользователей, владельцев групп и участников группы), либо динамически, в котором каждый пользователь просматривается руководителем или владельцами группы. Чтобы создать самообслуживайте (когда пользователи проверяют собственный доступ), не предоставьте рецензентов при создании [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .

Наследуется [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
| Свойство | Тип | Описание |
| :-------------------------| :---------- | :---------- |
| Запрос | Строка | Запрос, указывающий, кто будет рецензентом. Примеры см. в таблице. |
| queryType | Строка | Тип запроса. Примеры включают и `MicrosoftGraph` `ARM`. |
| queryRoot | String | В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для определения относительного источника запроса. Это свойство требуется только в том случае, если указан относительный запрос, `./manager`например. Возможное значение: `decisions`. |

Дополнительные сведения о параметрах конфигурации для рецензентов см. в статье "Назначение рецензентов определению проверки доступа [с помощью microsoft API Graph"](/graph/accessreviews-reviewers-concept).


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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
