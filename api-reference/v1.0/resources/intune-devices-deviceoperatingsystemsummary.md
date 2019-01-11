---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4b53d7c7260e58458995093bbea17df5464e704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846077"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="e523e-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e523e-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="e523e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e523e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e523e-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="e523e-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="e523e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e523e-106">Properties</span></span>
|<span data-ttu-id="e523e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e523e-107">Property</span></span>|<span data-ttu-id="e523e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e523e-108">Type</span></span>|<span data-ttu-id="e523e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e523e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e523e-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="e523e-110">androidCount</span></span>|<span data-ttu-id="e523e-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-111">Int32</span></span>|<span data-ttu-id="e523e-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="e523e-112">Number of android device count.</span></span>|
|<span data-ttu-id="e523e-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="e523e-113">iosCount</span></span>|<span data-ttu-id="e523e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-114">Int32</span></span>|<span data-ttu-id="e523e-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="e523e-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="e523e-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="e523e-116">macOSCount</span></span>|<span data-ttu-id="e523e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-117">Int32</span></span>|<span data-ttu-id="e523e-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="e523e-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="e523e-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="e523e-119">windowsMobileCount</span></span>|<span data-ttu-id="e523e-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-120">Int32</span></span>|<span data-ttu-id="e523e-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="e523e-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="e523e-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="e523e-122">windowsCount</span></span>|<span data-ttu-id="e523e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-123">Int32</span></span>|<span data-ttu-id="e523e-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="e523e-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="e523e-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e523e-125">unknownCount</span></span>|<span data-ttu-id="e523e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e523e-126">Int32</span></span>|<span data-ttu-id="e523e-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e523e-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e523e-128">Связи</span><span class="sxs-lookup"><span data-stu-id="e523e-128">Relationships</span></span>
<span data-ttu-id="e523e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="e523e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e523e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e523e-130">JSON Representation</span></span>
<span data-ttu-id="e523e-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e523e-131">Here is a JSON representation of the resource.</span></span>
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



