---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы проПускания
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba15df46075e5cbea1a2eab8a798c333f4a60ae6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178117"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="08449-103">Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="08449-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

> <span data-ttu-id="08449-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08449-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08449-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08449-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08449-106">Тип часов и процентного отношения для полосы проПускания</span><span class="sxs-lookup"><span data-stu-id="08449-106">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="08449-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08449-107">Properties</span></span>
|<span data-ttu-id="08449-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08449-108">Property</span></span>|<span data-ttu-id="08449-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08449-109">Type</span></span>|<span data-ttu-id="08449-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08449-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08449-111">Бандвидсбегинбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="08449-111">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="08449-112">Int32</span><span class="sxs-lookup"><span data-stu-id="08449-112">Int32</span></span>|<span data-ttu-id="08449-113">Указывает начало рабочего времени в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="08449-113">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="08449-114">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="08449-114">Valid values 0 to 23</span></span>|
|<span data-ttu-id="08449-115">Бандвидсендбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="08449-115">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="08449-116">Int32</span><span class="sxs-lookup"><span data-stu-id="08449-116">Int32</span></span>|<span data-ttu-id="08449-117">Задает время окончания рабочего дня в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="08449-117">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="08449-118">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="08449-118">Valid values 0 to 23</span></span>|
|<span data-ttu-id="08449-119">Бандвидсперцентажедурингбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="08449-119">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="08449-120">Int32</span><span class="sxs-lookup"><span data-stu-id="08449-120">Int32</span></span>|<span data-ttu-id="08449-121">Указывает процент пропускной способности для ограничения в рабочее время (0-100).</span><span class="sxs-lookup"><span data-stu-id="08449-121">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="08449-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="08449-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="08449-123">Бандвидсперцентажеаутсидебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="08449-123">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="08449-124">Int32</span><span class="sxs-lookup"><span data-stu-id="08449-124">Int32</span></span>|<span data-ttu-id="08449-125">Указывает процент пропускной способности, ограничивающий рабочие часы (0-100).</span><span class="sxs-lookup"><span data-stu-id="08449-125">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="08449-126">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="08449-126">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="08449-127">Связи</span><span class="sxs-lookup"><span data-stu-id="08449-127">Relationships</span></span>
<span data-ttu-id="08449-128">Нет</span><span class="sxs-lookup"><span data-stu-id="08449-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08449-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08449-129">JSON Representation</span></span>
<span data-ttu-id="08449-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08449-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```




