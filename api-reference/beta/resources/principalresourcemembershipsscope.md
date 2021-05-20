---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет для областей выбора просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b22c52c0bf71f1a1169d51e2e6fd3e8ac10e99d9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579895"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="c3a7d-103">тип ресурса principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="c3a7d-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="c3a7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="c3a7d-105">PrincipalResourceMembershipsScope — это тип [accessReviewScope,](accessreviewscope.md) который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и просмотреть доступ выбранных директоров к выбранным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="c3a7d-106">Он используется для настройки свойства **области** [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7d-106">It is used to configure the **scope** property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="c3a7d-107">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="c3a7d-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c3a7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3a7d-108">Properties</span></span>
|<span data-ttu-id="c3a7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3a7d-109">Property</span></span>|<span data-ttu-id="c3a7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3a7d-110">Type</span></span>|<span data-ttu-id="c3a7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a7d-112">principalScopes</span><span class="sxs-lookup"><span data-stu-id="c3a7d-112">principalScopes</span></span>|<span data-ttu-id="c3a7d-113">[коллекция accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7d-113">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="c3a7d-114">Определяет области, включаемые в обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-114">Defines the scopes of the principals to be included in an access review.</span></span>|
|<span data-ttu-id="c3a7d-115">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c3a7d-115">resourceScopes</span></span>|<span data-ttu-id="c3a7d-116">[коллекция accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7d-116">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="c3a7d-117">Определяет области ресурсов, для которых будет рассмотрен доступ.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-117">Defines the scopes of the resources for which access will be reviewed.</span></span>|

<span data-ttu-id="c3a7d-118">Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.principalResourceMembershipsScope` .</span><span class="sxs-lookup"><span data-stu-id="c3a7d-118">You must also specify the **@odata.type** type property with the value `#microsoft.graph.principalResourceMembershipsScope`.</span></span> <span data-ttu-id="c3a7d-119">Дополнительные информацию о  параметрах конфигурации области с помощью **principalResourceMembershipsScope** см. в меню Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-119">For more about configuration options for **scope** using **principalResourceMembershipsScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="c3a7d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3a7d-120">Relationships</span></span>
<span data-ttu-id="c3a7d-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3a7d-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3a7d-122">JSON representation</span></span>
<span data-ttu-id="c3a7d-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3a7d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
