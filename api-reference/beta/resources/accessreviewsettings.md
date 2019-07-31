---
title: Тип ресурса Акцессревиевсеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 2c51d94b3143d9929c03093cfb1a6625d6a9e3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974547"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="edc40-102">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="edc40-102">accessReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="edc40-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="edc40-103">Properties</span></span>
|<span data-ttu-id="edc40-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="edc40-104">Property</span></span>|<span data-ttu-id="edc40-105">Тип</span><span class="sxs-lookup"><span data-stu-id="edc40-105">Type</span></span>|<span data-ttu-id="edc40-106">Описание</span><span class="sxs-lookup"><span data-stu-id="edc40-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="edc40-107">Маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="edc40-107">mailNotificationsEnabled</span></span> | <span data-ttu-id="edc40-108">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-108">boolean</span></span> |  |
| <span data-ttu-id="edc40-109">Реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="edc40-109">remindersEnabled</span></span> | <span data-ttu-id="edc40-110">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-110">boolean</span></span> |  |
| <span data-ttu-id="edc40-111">Жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="edc40-111">justificationRequiredOnApproval</span></span> | <span data-ttu-id="edc40-112">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-112">boolean</span></span> |  |
| <span data-ttu-id="edc40-113">Рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="edc40-113">recurrenceSettings</span></span> | <span data-ttu-id="edc40-114">Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="edc40-114">accessReviewRecurrenceSettings</span></span> |  |
| <span data-ttu-id="edc40-115">Ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="edc40-115">autoReviewEnabled</span></span> | <span data-ttu-id="edc40-116">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-116">boolean</span></span> |  |
| <span data-ttu-id="edc40-117">Активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="edc40-117">activityDurationInDays</span></span> | <span data-ttu-id="edc40-118">Int32</span><span class="sxs-lookup"><span data-stu-id="edc40-118">Int32</span></span> |  |
| <span data-ttu-id="edc40-119">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="edc40-119">autoReviewSettings</span></span> | <span data-ttu-id="edc40-120">Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="edc40-120">autoReviewSettings</span></span> |  |
| <span data-ttu-id="edc40-121">Аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="edc40-121">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="edc40-122">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-122">boolean</span></span> |  |
| <span data-ttu-id="edc40-123">Акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="edc40-123">accessRecommendationsEnabled</span></span> | <span data-ttu-id="edc40-124">boolean</span><span class="sxs-lookup"><span data-stu-id="edc40-124">boolean</span></span> |  |


## <a name="relationships"></a><span data-ttu-id="edc40-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="edc40-125">Relationships</span></span>
<span data-ttu-id="edc40-126">Нет</span><span class="sxs-lookup"><span data-stu-id="edc40-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="edc40-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edc40-127">JSON Representation</span></span>
<span data-ttu-id="edc40-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edc40-128">Here is a JSON representation of the resource.</span></span>
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



