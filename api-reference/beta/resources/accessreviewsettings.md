---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 21915811da771bd0eebdb5fb2c16df5cfbdea096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508459"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="b0889-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b0889-102">accessReviewSettings resource type</span></span>

<span data-ttu-id="b0889-103">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0889-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="b0889-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0889-104">Properties</span></span>
|<span data-ttu-id="b0889-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0889-105">Property</span></span>|<span data-ttu-id="b0889-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b0889-106">Type</span></span>|<span data-ttu-id="b0889-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b0889-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="b0889-108">маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b0889-108">mailNotificationsEnabled</span></span> | <span data-ttu-id="b0889-109">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-109">boolean</span></span> |  |
| <span data-ttu-id="b0889-110">реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="b0889-110">remindersEnabled</span></span> | <span data-ttu-id="b0889-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-111">boolean</span></span> |  |
| <span data-ttu-id="b0889-112">жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="b0889-112">justificationRequiredOnApproval</span></span> | <span data-ttu-id="b0889-113">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-113">boolean</span></span> |  |
| <span data-ttu-id="b0889-114">рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b0889-114">recurrenceSettings</span></span> | <span data-ttu-id="b0889-115">акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="b0889-115">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="b0889-116">ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="b0889-116">autoReviewEnabled</span></span> | <span data-ttu-id="b0889-117">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-117">boolean</span></span> |  |
| <span data-ttu-id="b0889-118">активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="b0889-118">activityDurationInDays</span></span> | <span data-ttu-id="b0889-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b0889-119">Int32</span></span> |  |
| <span data-ttu-id="b0889-120">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b0889-120">autoReviewSettings</span></span> | <span data-ttu-id="b0889-121">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="b0889-121">autoReviewSettings</span></span> |  |
| <span data-ttu-id="b0889-122">аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="b0889-122">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="b0889-123">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-123">boolean</span></span> |  |
| <span data-ttu-id="b0889-124">акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="b0889-124">accessRecommendationsEnabled</span></span> | <span data-ttu-id="b0889-125">boolean</span><span class="sxs-lookup"><span data-stu-id="b0889-125">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="b0889-126">Связи</span><span class="sxs-lookup"><span data-stu-id="b0889-126">Relationships</span></span>
<span data-ttu-id="b0889-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b0889-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0889-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0889-128">JSON Representation</span></span>
<span data-ttu-id="b0889-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0889-129">Here is a JSON representation of the resource.</span></span>
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



