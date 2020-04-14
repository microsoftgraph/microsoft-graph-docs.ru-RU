---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 978b8f80b6a357ffeb2efced005e395787fedabf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457097"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="b625e-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b625e-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="b625e-103">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b625e-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="b625e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b625e-104">Properties</span></span>
|<span data-ttu-id="b625e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b625e-105">Property</span></span>|<span data-ttu-id="b625e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b625e-106">Type</span></span>|<span data-ttu-id="b625e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b625e-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="b625e-108">маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b625e-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="b625e-109">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-109">boolean</span></span> |  |
| <span data-ttu-id="b625e-110">реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="b625e-110">remindersEnabled</span></span> | <span data-ttu-id="b625e-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-111">boolean</span></span> |  |
| <span data-ttu-id="b625e-112">жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="b625e-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="b625e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-113">boolean</span></span> |  |
| <span data-ttu-id="b625e-114">рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b625e-114">recurrenceSettings</span></span> | <span data-ttu-id="b625e-115">акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b625e-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="b625e-116">ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="b625e-116">autoReviewEnabled</span></span> | <span data-ttu-id="b625e-117">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-117">boolean</span></span> |  |
| <span data-ttu-id="b625e-118">активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="b625e-118">activityDurationInDays</span></span> | <span data-ttu-id="b625e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b625e-119">Int32</span></span> |  |
| <span data-ttu-id="b625e-120">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b625e-120">autoReviewSettings</span></span> | <span data-ttu-id="b625e-121">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b625e-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="b625e-122">аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="b625e-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="b625e-123">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-123">boolean</span></span> |  |
| <span data-ttu-id="b625e-124">акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b625e-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="b625e-125">boolean</span><span class="sxs-lookup"><span data-stu-id="b625e-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="b625e-126">Связи</span><span class="sxs-lookup"><span data-stu-id="b625e-126">Relationships</span></span>
<span data-ttu-id="b625e-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b625e-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b625e-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b625e-128">JSON Representation</span></span>
<span data-ttu-id="b625e-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b625e-129">Here is a JSON representation of the resource.</span></span>
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



