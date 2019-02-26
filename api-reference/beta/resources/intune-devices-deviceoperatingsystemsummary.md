---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3cf55de11b4d8610cb0622eca9ab740a6b2a40b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157304"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="2e37e-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2e37e-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="2e37e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e37e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e37e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e37e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e37e-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="2e37e-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="2e37e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e37e-107">Properties</span></span>
|<span data-ttu-id="2e37e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e37e-108">Property</span></span>|<span data-ttu-id="2e37e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e37e-109">Type</span></span>|<span data-ttu-id="2e37e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e37e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e37e-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-111">androidCount</span></span>|<span data-ttu-id="2e37e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-112">Int32</span></span>|<span data-ttu-id="2e37e-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="2e37e-113">Number of android device count.</span></span>|
|<span data-ttu-id="2e37e-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-114">iosCount</span></span>|<span data-ttu-id="2e37e-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-115">Int32</span></span>|<span data-ttu-id="2e37e-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="2e37e-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="2e37e-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-117">macOSCount</span></span>|<span data-ttu-id="2e37e-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-118">Int32</span></span>|<span data-ttu-id="2e37e-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="2e37e-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="2e37e-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-120">windowsMobileCount</span></span>|<span data-ttu-id="2e37e-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-121">Int32</span></span>|<span data-ttu-id="2e37e-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2e37e-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="2e37e-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-123">windowsCount</span></span>|<span data-ttu-id="2e37e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-124">Int32</span></span>|<span data-ttu-id="2e37e-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="2e37e-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="2e37e-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="2e37e-126">unknownCount</span></span>|<span data-ttu-id="2e37e-127">Int32</span><span class="sxs-lookup"><span data-stu-id="2e37e-127">Int32</span></span>|<span data-ttu-id="2e37e-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="2e37e-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e37e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="2e37e-129">Relationships</span></span>
<span data-ttu-id="2e37e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="2e37e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e37e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e37e-131">JSON Representation</span></span>
<span data-ttu-id="2e37e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e37e-132">Here is a JSON representation of the resource.</span></span>
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




