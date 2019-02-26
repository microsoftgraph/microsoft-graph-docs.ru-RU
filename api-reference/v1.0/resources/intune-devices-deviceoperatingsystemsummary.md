---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250406"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="2a635-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2a635-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="2a635-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a635-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a635-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="2a635-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="2a635-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a635-106">Properties</span></span>
|<span data-ttu-id="2a635-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a635-107">Property</span></span>|<span data-ttu-id="2a635-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2a635-108">Type</span></span>|<span data-ttu-id="2a635-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a635-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a635-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="2a635-110">androidCount</span></span>|<span data-ttu-id="2a635-111">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-111">Int32</span></span>|<span data-ttu-id="2a635-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="2a635-112">Number of android device count.</span></span>|
|<span data-ttu-id="2a635-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="2a635-113">iosCount</span></span>|<span data-ttu-id="2a635-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-114">Int32</span></span>|<span data-ttu-id="2a635-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="2a635-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="2a635-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="2a635-116">macOSCount</span></span>|<span data-ttu-id="2a635-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-117">Int32</span></span>|<span data-ttu-id="2a635-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="2a635-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="2a635-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="2a635-119">windowsMobileCount</span></span>|<span data-ttu-id="2a635-120">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-120">Int32</span></span>|<span data-ttu-id="2a635-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2a635-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="2a635-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="2a635-122">windowsCount</span></span>|<span data-ttu-id="2a635-123">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-123">Int32</span></span>|<span data-ttu-id="2a635-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2a635-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="2a635-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="2a635-125">unknownCount</span></span>|<span data-ttu-id="2a635-126">Int32</span><span class="sxs-lookup"><span data-stu-id="2a635-126">Int32</span></span>|<span data-ttu-id="2a635-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="2a635-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a635-128">Связи</span><span class="sxs-lookup"><span data-stu-id="2a635-128">Relationships</span></span>
<span data-ttu-id="2a635-129">Нет</span><span class="sxs-lookup"><span data-stu-id="2a635-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a635-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a635-130">JSON Representation</span></span>
<span data-ttu-id="2a635-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a635-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



