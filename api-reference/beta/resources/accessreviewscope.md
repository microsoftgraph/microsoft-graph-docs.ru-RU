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
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="6f158-103">тип ресурса accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="6f158-103">accessReviewScope resource type</span></span>

<span data-ttu-id="6f158-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f158-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="6f158-105">**AccessReviewScope** определяет, какие объекты будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6f158-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="6f158-106">Это абстрактный тип, унаследованный [accessReviewQueryScope,](accessreviewqueryscope.md) [principalResourceMembershipsScope](principalresourcemembershipsscope.md) и [accessReviewReviewerScope.](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="6f158-106">It is an abstract type that is inherited by [accessReviewQueryScope](accessreviewqueryscope.md), [principalResourceMembershipsScope](principalresourcemembershipsscope.md) and [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> 

<span data-ttu-id="6f158-107">Для `scope` свойства в [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) см. [accessReviewQueryScope](accessreviewqueryscope.md) и [principalResourceMembershipsScope.](principalresourcemembershipsscope.md)</span><span class="sxs-lookup"><span data-stu-id="6f158-107">For `scope` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewQueryScope](accessreviewqueryscope.md) and [principalResourceMembershipsScope](principalresourcemembershipsscope.md).</span></span>

<span data-ttu-id="6f158-108">Свойства `reviewers` в [accessReviewScheduleDefinition см.](accessreviewscheduledefinition.md) [в разделах accessReviewReviewerScope](accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="6f158-108">For `reviewers` property on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) see [accessReviewReviewerScope](accessreviewreviewerscope.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f158-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f158-109">Properties</span></span>
<span data-ttu-id="6f158-110">Нет</span><span class="sxs-lookup"><span data-stu-id="6f158-110">None.</span></span>


## <a name="relationships"></a><span data-ttu-id="6f158-111">Связи</span><span class="sxs-lookup"><span data-stu-id="6f158-111">Relationships</span></span>
<span data-ttu-id="6f158-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6f158-112">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f158-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6f158-113">JSON representation</span></span>
<span data-ttu-id="6f158-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f158-114">The following is a JSON representation of the resource.</span></span>
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
