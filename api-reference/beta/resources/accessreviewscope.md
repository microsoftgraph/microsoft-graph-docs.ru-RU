---
title: тип ресурса accessReviewScope
description: 'В функции обзоров доступа Azure AD представлены объекты, которые будут рассмотрены `accessReviewScope` в обзоре доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0888aa8666f3335a42dc6686531f88fd0f3325ed
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579727"
---
# <a name="accessreviewscope-resource-type"></a>тип ресурса accessReviewScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

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
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
