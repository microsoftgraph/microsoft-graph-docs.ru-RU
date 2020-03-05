---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы пропускной способности, указанные в процентах.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85053c5e02b9ac429a3251c1c302c786f6a8f6db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526796"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="d4e17-103">Тип ресурса Деливерйоптимизатионбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="d4e17-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="d4e17-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4e17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e17-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4e17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e17-107">Пределы пропускной способности, указанные в процентах.</span><span class="sxs-lookup"><span data-stu-id="d4e17-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="d4e17-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="d4e17-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4e17-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4e17-109">Properties</span></span>
|<span data-ttu-id="d4e17-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4e17-110">Property</span></span>|<span data-ttu-id="d4e17-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d4e17-111">Type</span></span>|<span data-ttu-id="d4e17-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e17-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e17-113">максимумбаккграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="d4e17-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="d4e17-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e17-114">Int32</span></span>|<span data-ttu-id="d4e17-115">Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="d4e17-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="d4e17-116">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="d4e17-116">Valid values 0 to 100</span></span>
<span data-ttu-id="d4e17-117">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="d4e17-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="d4e17-118">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="d4e17-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d4e17-119">максимумфореграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="d4e17-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="d4e17-120">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e17-120">Int32</span></span>|<span data-ttu-id="d4e17-121">Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="d4e17-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="d4e17-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="d4e17-122">Valid values 0 to 100</span></span>
<span data-ttu-id="d4e17-123">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="d4e17-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="d4e17-124">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="d4e17-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4e17-125">Связи</span><span class="sxs-lookup"><span data-stu-id="d4e17-125">Relationships</span></span>
<span data-ttu-id="d4e17-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d4e17-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4e17-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4e17-127">JSON Representation</span></span>
<span data-ttu-id="d4e17-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e17-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```



