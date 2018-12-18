---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
ms.openlocfilehash: 73615964d0c2b187c36b57956d534fa08d60684f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346622"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="aa9df-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="aa9df-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="aa9df-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa9df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa9df-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="aa9df-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="aa9df-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa9df-106">Properties</span></span>
|<span data-ttu-id="aa9df-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa9df-107">Property</span></span>|<span data-ttu-id="aa9df-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa9df-108">Type</span></span>|<span data-ttu-id="aa9df-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa9df-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa9df-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-110">androidCount</span></span>|<span data-ttu-id="aa9df-111">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-111">Int32</span></span>|<span data-ttu-id="aa9df-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="aa9df-112">Number of android device count.</span></span>|
|<span data-ttu-id="aa9df-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-113">iosCount</span></span>|<span data-ttu-id="aa9df-114">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-114">Int32</span></span>|<span data-ttu-id="aa9df-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="aa9df-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="aa9df-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-116">macOSCount</span></span>|<span data-ttu-id="aa9df-117">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-117">Int32</span></span>|<span data-ttu-id="aa9df-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="aa9df-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="aa9df-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-119">windowsMobileCount</span></span>|<span data-ttu-id="aa9df-120">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-120">Int32</span></span>|<span data-ttu-id="aa9df-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="aa9df-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="aa9df-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-122">windowsCount</span></span>|<span data-ttu-id="aa9df-123">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-123">Int32</span></span>|<span data-ttu-id="aa9df-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="aa9df-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="aa9df-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="aa9df-125">unknownCount</span></span>|<span data-ttu-id="aa9df-126">Int32</span><span class="sxs-lookup"><span data-stu-id="aa9df-126">Int32</span></span>|<span data-ttu-id="aa9df-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="aa9df-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa9df-128">Связи</span><span class="sxs-lookup"><span data-stu-id="aa9df-128">Relationships</span></span>
<span data-ttu-id="aa9df-129">Нет</span><span class="sxs-lookup"><span data-stu-id="aa9df-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa9df-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa9df-130">JSON Representation</span></span>
<span data-ttu-id="aa9df-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa9df-131">Here is a JSON representation of the resource.</span></span>
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



