---
title: Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит
description: Тип часов и процентного отношения для полосы пропускания
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1284062e20df896dd30a99bec5506ad101c742ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526812"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a><span data-ttu-id="99652-103">Тип ресурса Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="99652-103">deliveryOptimizationBandwidthBusinessHoursLimit resource type</span></span>

<span data-ttu-id="99652-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="99652-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99652-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99652-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99652-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99652-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99652-107">Тип часов и процентного отношения для полосы пропускания</span><span class="sxs-lookup"><span data-stu-id="99652-107">Bandwidth business hours and percentages type</span></span>

## <a name="properties"></a><span data-ttu-id="99652-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="99652-108">Properties</span></span>
|<span data-ttu-id="99652-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="99652-109">Property</span></span>|<span data-ttu-id="99652-110">Тип</span><span class="sxs-lookup"><span data-stu-id="99652-110">Type</span></span>|<span data-ttu-id="99652-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99652-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99652-112">бандвидсбегинбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="99652-112">bandwidthBeginBusinessHours</span></span>|<span data-ttu-id="99652-113">Int32</span><span class="sxs-lookup"><span data-stu-id="99652-113">Int32</span></span>|<span data-ttu-id="99652-114">Указывает начало рабочего времени в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="99652-114">Specifies the beginning of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="99652-115">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="99652-115">Valid values 0 to 23</span></span>|
|<span data-ttu-id="99652-116">бандвидсендбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="99652-116">bandwidthEndBusinessHours</span></span>|<span data-ttu-id="99652-117">Int32</span><span class="sxs-lookup"><span data-stu-id="99652-117">Int32</span></span>|<span data-ttu-id="99652-118">Задает время окончания рабочего дня в 24-часовом формате (0-23).</span><span class="sxs-lookup"><span data-stu-id="99652-118">Specifies the end of business hours using a 24-hour clock (0-23).</span></span> <span data-ttu-id="99652-119">Допустимые значения — от 0 до 23.</span><span class="sxs-lookup"><span data-stu-id="99652-119">Valid values 0 to 23</span></span>|
|<span data-ttu-id="99652-120">бандвидсперцентажедурингбусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="99652-120">bandwidthPercentageDuringBusinessHours</span></span>|<span data-ttu-id="99652-121">Int32</span><span class="sxs-lookup"><span data-stu-id="99652-121">Int32</span></span>|<span data-ttu-id="99652-122">Указывает процент пропускной способности для ограничения в рабочее время (0-100).</span><span class="sxs-lookup"><span data-stu-id="99652-122">Specifies the percentage of bandwidth to limit during business hours (0-100).</span></span> <span data-ttu-id="99652-123">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="99652-123">Valid values 0 to 100</span></span>|
|<span data-ttu-id="99652-124">бандвидсперцентажеаутсидебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="99652-124">bandwidthPercentageOutsideBusinessHours</span></span>|<span data-ttu-id="99652-125">Int32</span><span class="sxs-lookup"><span data-stu-id="99652-125">Int32</span></span>|<span data-ttu-id="99652-126">Указывает процент пропускной способности, ограничивающий рабочие часы (0-100).</span><span class="sxs-lookup"><span data-stu-id="99652-126">Specifies the percentage of bandwidth to limit outsidse business hours (0-100).</span></span> <span data-ttu-id="99652-127">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="99652-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="99652-128">Связи</span><span class="sxs-lookup"><span data-stu-id="99652-128">Relationships</span></span>
<span data-ttu-id="99652-129">Нет</span><span class="sxs-lookup"><span data-stu-id="99652-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99652-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99652-130">JSON Representation</span></span>
<span data-ttu-id="99652-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99652-131">Here is a JSON representation of the resource.</span></span>
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



