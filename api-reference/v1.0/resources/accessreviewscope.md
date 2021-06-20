---
title: тип ресурса accessReviewScope
description: Представляет объекты, которые необходимо просмотреть в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d377bfbf9a69c71d7349724863438ab31ddbe6b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031234"
---
# <a name="accessreviewscope-resource-type"></a>тип ресурса accessReviewScope

Пространство имен: microsoft.graph

**AccessReviewScope** определяет, какие объекты будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это абстрактный тип, унаследованный [accessReviewQueryScope,](accessreviewqueryscope.md) [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewReviewerScope.](accessreviewreviewerscope.md) 

Для **свойства области** в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewQueryScope](accessreviewqueryscope.md) и [principalResourceMembershipsScope.](principalresourcemembershipsscope.md)

Для **свойства рецензентов** в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewReviewerScope.](accessreviewreviewerscope.md)

Указание типа OData в  области настоятельно рекомендуется для всех типов, но необходимо для [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).

## <a name="properties"></a>Свойства
Нет


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
