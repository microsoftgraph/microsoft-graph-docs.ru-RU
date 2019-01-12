---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975647"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="5fee5-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="5fee5-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="5fee5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5fee5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fee5-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="5fee5-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="5fee5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fee5-106">Properties</span></span>
|<span data-ttu-id="5fee5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fee5-107">Property</span></span>|<span data-ttu-id="5fee5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5fee5-108">Type</span></span>|<span data-ttu-id="5fee5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5fee5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fee5-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-110">androidCount</span></span>|<span data-ttu-id="5fee5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-111">Int32</span></span>|<span data-ttu-id="5fee5-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="5fee5-112">Number of android device count.</span></span>|
|<span data-ttu-id="5fee5-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-113">iosCount</span></span>|<span data-ttu-id="5fee5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-114">Int32</span></span>|<span data-ttu-id="5fee5-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="5fee5-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="5fee5-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-116">macOSCount</span></span>|<span data-ttu-id="5fee5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-117">Int32</span></span>|<span data-ttu-id="5fee5-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="5fee5-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="5fee5-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-119">windowsMobileCount</span></span>|<span data-ttu-id="5fee5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-120">Int32</span></span>|<span data-ttu-id="5fee5-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="5fee5-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="5fee5-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-122">windowsCount</span></span>|<span data-ttu-id="5fee5-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-123">Int32</span></span>|<span data-ttu-id="5fee5-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="5fee5-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="5fee5-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="5fee5-125">unknownCount</span></span>|<span data-ttu-id="5fee5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5fee5-126">Int32</span></span>|<span data-ttu-id="5fee5-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="5fee5-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fee5-128">Связи</span><span class="sxs-lookup"><span data-stu-id="5fee5-128">Relationships</span></span>
<span data-ttu-id="5fee5-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5fee5-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5fee5-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fee5-130">JSON Representation</span></span>
<span data-ttu-id="5fee5-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fee5-131">Here is a JSON representation of the resource.</span></span>
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



