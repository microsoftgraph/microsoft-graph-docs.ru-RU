---
title: тип ресурса accessReviewScope
description: Представляет объекты, которые необходимо просмотреть в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9194d0b07c2b24d37f811c2348ed7b4b1a8498e2f592b6a10d97dc212d180be9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121447"
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
