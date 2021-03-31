---
title: тип ресурса accessReviewScope
description: 'В функции обзоров доступа Azure AD представлены объекты, которые будут рассмотрены `accessReviewScope` в обзоре доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04955ba6980dd94995da1610afcc1e33046e4473
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469313"
---
# <a name="accessreviewscope-resource-type"></a>тип ресурса accessReviewScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**AccessReviewScope** определяет, какие объекты будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md) Это абстрактный тип, унаследованный [accessReviewQueryScope,](accessreviewqueryscope.md) [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewReviewerScope.](accessreviewreviewerscope.md) 

Для `scope` свойства в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewQueryScope](accessreviewqueryscope.md) и [principalResourceMembershipsScope.](principalresourcemembershipsscope.md)

Свойства `reviewers` в [accessReviewScheduleDefinition см.](accessreviewscheduledefinition.md) [в разделах accessReviewReviewerScope](accessreviewreviewerscope.md)

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
