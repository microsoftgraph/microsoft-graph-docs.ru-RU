---
title: Тип ресурса accessReviewScope
description: Представляет сущности, которые необходимо проверить при проверке доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f14589faad21b586fb3dcc2c6f8b16be9da84f03
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698431"
---
# <a name="accessreviewscope-resource-type"></a>Тип ресурса accessReviewScope

Пространство имен: microsoft.graph

**AccessReviewScope** определяет, какие сущности проверяются в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Это абстрактный тип, наследуемый [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewReviewerScope](accessreviewreviewerscope.md). 

Сведения **о свойстве** scope в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. в [разделе accessReviewQueryScope](accessreviewqueryscope.md) и [principalResourceMembershipsScope](principalresourcemembershipsscope.md).

Сведения **о свойстве** рецензентов [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [в разделе accessReviewReviewerScope](accessreviewreviewerscope.md).

Указание типа OData в области настоятельно рекомендуется  для всех типов, но требуется для [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).

## <a name="properties"></a>Свойства
Нет


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope"
}
```
