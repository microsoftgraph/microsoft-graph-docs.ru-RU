---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348424"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="3e08a-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3e08a-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="3e08a-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e08a-103">Properties</span></span>
|<span data-ttu-id="3e08a-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e08a-104">Property</span></span>|<span data-ttu-id="3e08a-105">Тип</span><span class="sxs-lookup"><span data-stu-id="3e08a-105">Type</span></span>|<span data-ttu-id="3e08a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="3e08a-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="3e08a-107">Маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="3e08a-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="3e08a-108">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-108">boolean</span></span> |  |
| <span data-ttu-id="3e08a-109">Реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="3e08a-109">remindersEnabled</span></span> | <span data-ttu-id="3e08a-110">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-110">boolean</span></span> |  |
| <span data-ttu-id="3e08a-111">Жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="3e08a-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="3e08a-112">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-112">boolean</span></span> |  |
| <span data-ttu-id="3e08a-113">Рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="3e08a-113">recurrenceSettings</span></span> | <span data-ttu-id="3e08a-114">Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="3e08a-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="3e08a-115">Ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="3e08a-115">autoReviewEnabled</span></span> | <span data-ttu-id="3e08a-116">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-116">boolean</span></span> |  |
| <span data-ttu-id="3e08a-117">Активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="3e08a-117">activityDurationInDays</span></span> | <span data-ttu-id="3e08a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3e08a-118">Int32</span></span> |  |
| <span data-ttu-id="3e08a-119">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3e08a-119">autoReviewSettings</span></span> | <span data-ttu-id="3e08a-120">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="3e08a-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="3e08a-121">Аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="3e08a-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="3e08a-122">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-122">boolean</span></span> |  |
| <span data-ttu-id="3e08a-123">Акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="3e08a-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="3e08a-124">boolean</span><span class="sxs-lookup"><span data-stu-id="3e08a-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="3e08a-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="3e08a-125">Relationships</span></span>
<span data-ttu-id="3e08a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3e08a-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e08a-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e08a-127">JSON Representation</span></span>
<span data-ttu-id="3e08a-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e08a-128">Here is a JSON representation of the resource.</span></span>
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



