---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
ms.openlocfilehash: 1a543f21d1f82b9f2bee0f004d3b8fab88c863b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026692"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="293bf-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="293bf-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="293bf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="293bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="293bf-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="293bf-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="293bf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="293bf-106">Properties</span></span>
|<span data-ttu-id="293bf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="293bf-107">Property</span></span>|<span data-ttu-id="293bf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="293bf-108">Type</span></span>|<span data-ttu-id="293bf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="293bf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293bf-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="293bf-110">androidCount</span></span>|<span data-ttu-id="293bf-111">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-111">Int32</span></span>|<span data-ttu-id="293bf-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="293bf-112">Number of android device count.</span></span>|
|<span data-ttu-id="293bf-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="293bf-113">iosCount</span></span>|<span data-ttu-id="293bf-114">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-114">Int32</span></span>|<span data-ttu-id="293bf-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="293bf-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="293bf-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="293bf-116">macOSCount</span></span>|<span data-ttu-id="293bf-117">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-117">Int32</span></span>|<span data-ttu-id="293bf-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="293bf-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="293bf-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="293bf-119">windowsMobileCount</span></span>|<span data-ttu-id="293bf-120">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-120">Int32</span></span>|<span data-ttu-id="293bf-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="293bf-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="293bf-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="293bf-122">windowsCount</span></span>|<span data-ttu-id="293bf-123">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-123">Int32</span></span>|<span data-ttu-id="293bf-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="293bf-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="293bf-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="293bf-125">unknownCount</span></span>|<span data-ttu-id="293bf-126">Int32</span><span class="sxs-lookup"><span data-stu-id="293bf-126">Int32</span></span>|<span data-ttu-id="293bf-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="293bf-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="293bf-128">Связи</span><span class="sxs-lookup"><span data-stu-id="293bf-128">Relationships</span></span>
<span data-ttu-id="293bf-129">Нет</span><span class="sxs-lookup"><span data-stu-id="293bf-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="293bf-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="293bf-130">JSON Representation</span></span>
<span data-ttu-id="293bf-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="293bf-131">Here is a JSON representation of the resource.</span></span>
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



