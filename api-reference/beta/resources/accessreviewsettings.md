---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084070"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="b85c0-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b85c0-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="b85c0-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="b85c0-103">Properties</span></span>
|<span data-ttu-id="b85c0-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="b85c0-104">Property</span></span>|<span data-ttu-id="b85c0-105">Тип</span><span class="sxs-lookup"><span data-stu-id="b85c0-105">Type</span></span>|<span data-ttu-id="b85c0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b85c0-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="b85c0-107">Маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b85c0-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="b85c0-108">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-108">boolean</span></span> |  |
| <span data-ttu-id="b85c0-109">Реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="b85c0-109">remindersEnabled</span></span> | <span data-ttu-id="b85c0-110">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-110">boolean</span></span> |  |
| <span data-ttu-id="b85c0-111">Жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="b85c0-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="b85c0-112">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-112">boolean</span></span> |  |
| <span data-ttu-id="b85c0-113">Рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b85c0-113">recurrenceSettings</span></span> | <span data-ttu-id="b85c0-114">Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b85c0-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="b85c0-115">Ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="b85c0-115">autoReviewEnabled</span></span> | <span data-ttu-id="b85c0-116">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-116">boolean</span></span> |  |
| <span data-ttu-id="b85c0-117">Активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="b85c0-117">activityDurationInDays</span></span> | <span data-ttu-id="b85c0-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b85c0-118">Int32</span></span> |  |
| <span data-ttu-id="b85c0-119">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b85c0-119">autoReviewSettings</span></span> | <span data-ttu-id="b85c0-120">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b85c0-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="b85c0-121">Аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="b85c0-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="b85c0-122">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-122">boolean</span></span> |  |
| <span data-ttu-id="b85c0-123">Акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b85c0-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="b85c0-124">boolean</span><span class="sxs-lookup"><span data-stu-id="b85c0-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="b85c0-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="b85c0-125">Relationships</span></span>
<span data-ttu-id="b85c0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b85c0-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b85c0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b85c0-127">JSON Representation</span></span>
<span data-ttu-id="b85c0-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b85c0-128">Here is a JSON representation of the resource.</span></span>
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



