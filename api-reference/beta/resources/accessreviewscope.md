---
title: Тип ресурса accessReviewScope
description: 'В Azure AD проверки доступа эта функция представляет сущности, `accessReviewScope` которые будут проверяться при проверке доступа.  '
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa4d8dd9db5fa16736552acbed2c9e59592980af
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698113"
---
# <a name="accessreviewscope-resource-type"></a>Тип ресурса accessReviewScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

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
