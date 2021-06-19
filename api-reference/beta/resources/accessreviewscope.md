---
title: тип ресурса accessReviewScope
description: 'В функции обзоров доступа Azure AD представлены объекты, которые будут рассмотрены `accessReviewScope` в обзоре доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84b427cdd05aa35fdacb6b80d6ac96c901eef318
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030924"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="98459-103">тип ресурса accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="98459-103">accessReviewScope resource type</span></span>

<span data-ttu-id="98459-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98459-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="98459-105">**AccessReviewScope** определяет, какие объекты будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="98459-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="98459-106">Это абстрактный тип, унаследованный [accessReviewQueryScope,](accessreviewqueryscope.md) [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewReviewerScope.](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="98459-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="98459-107">Для **свойства области** в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewQueryScope](accessreviewqueryscope.md) и [principalResourceMembershipsScope.](principalresourcemembershipsscope.md)</span><span class="sxs-lookup"><span data-stu-id="98459-107">For **scope** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="98459-108">Для **свойства рецензентов** в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewReviewerScope.](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="98459-108">For **reviewers** property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span>

<span data-ttu-id="98459-109">Указание типа OData в  области настоятельно рекомендуется для всех типов, но необходимо для [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="98459-109">Specifying the OData type in the **scope** is highly recommended for all types but required for [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="98459-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="98459-110">Properties</span></span>
<span data-ttu-id="98459-111">Нет</span><span class="sxs-lookup"><span data-stu-id="98459-111">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="98459-112">Связи</span><span class="sxs-lookup"><span data-stu-id="98459-112">Relationships</span></span>
<span data-ttu-id="98459-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98459-113">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98459-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98459-114">JSON representation</span></span>
<span data-ttu-id="98459-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98459-115">The following is a JSON representation of the resource.</span></span>
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
