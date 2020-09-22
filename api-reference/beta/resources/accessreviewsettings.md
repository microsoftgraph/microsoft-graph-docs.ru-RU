---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 201f0c0ac11a0e26174661aa4d8a63baf23f7f3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024572"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="3ed5c-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="3ed5c-103">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed5c-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="3ed5c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ed5c-104">Properties</span></span>
|<span data-ttu-id="3ed5c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ed5c-105">Property</span></span>|<span data-ttu-id="3ed5c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3ed5c-106">Type</span></span>|<span data-ttu-id="3ed5c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="3ed5c-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="3ed5c-108">маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="3ed5c-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="3ed5c-109">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-109">boolean</span></span> |  |
| <span data-ttu-id="3ed5c-110">реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="3ed5c-110">remindersEnabled</span></span> | <span data-ttu-id="3ed5c-111">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-111">boolean</span></span> |  |
| <span data-ttu-id="3ed5c-112">жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="3ed5c-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="3ed5c-113">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-113">boolean</span></span> |  |
| <span data-ttu-id="3ed5c-114">рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-114">recurrenceSettings</span></span> | <span data-ttu-id="3ed5c-115">акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="3ed5c-116">ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="3ed5c-116">autoReviewEnabled</span></span> | <span data-ttu-id="3ed5c-117">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-117">boolean</span></span> |  |
| <span data-ttu-id="3ed5c-118">активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-118">activityDurationInDays</span></span> | <span data-ttu-id="3ed5c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3ed5c-119">Int32</span></span> |  |
| <span data-ttu-id="3ed5c-120">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-120">autoReviewSettings</span></span> | <span data-ttu-id="3ed5c-121">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3ed5c-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="3ed5c-122">аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="3ed5c-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="3ed5c-123">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-123">boolean</span></span> |  |
| <span data-ttu-id="3ed5c-124">акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="3ed5c-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="3ed5c-125">boolean</span><span class="sxs-lookup"><span data-stu-id="3ed5c-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="3ed5c-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ed5c-126">Relationships</span></span>
<span data-ttu-id="3ed5c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="3ed5c-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ed5c-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ed5c-128">JSON Representation</span></span>
<span data-ttu-id="3ed5c-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ed5c-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```





