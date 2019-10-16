---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccb18fa2f8ec1545530dca13a7ed9d59be5a7504
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539101"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="93f1f-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="93f1f-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="93f1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93f1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93f1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f1f-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="93f1f-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="93f1f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="93f1f-107">Properties</span></span>
|<span data-ttu-id="93f1f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="93f1f-108">Property</span></span>|<span data-ttu-id="93f1f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="93f1f-109">Type</span></span>|<span data-ttu-id="93f1f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93f1f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f1f-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-111">androidCount</span></span>|<span data-ttu-id="93f1f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-112">Int32</span></span>|<span data-ttu-id="93f1f-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="93f1f-113">Number of android device count.</span></span>|
|<span data-ttu-id="93f1f-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-114">iosCount</span></span>|<span data-ttu-id="93f1f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-115">Int32</span></span>|<span data-ttu-id="93f1f-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="93f1f-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="93f1f-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-117">macOSCount</span></span>|<span data-ttu-id="93f1f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-118">Int32</span></span>|<span data-ttu-id="93f1f-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="93f1f-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="93f1f-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-120">windowsMobileCount</span></span>|<span data-ttu-id="93f1f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-121">Int32</span></span>|<span data-ttu-id="93f1f-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="93f1f-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="93f1f-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-123">windowsCount</span></span>|<span data-ttu-id="93f1f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-124">Int32</span></span>|<span data-ttu-id="93f1f-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="93f1f-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="93f1f-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="93f1f-126">unknownCount</span></span>|<span data-ttu-id="93f1f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-127">Int32</span></span>|<span data-ttu-id="93f1f-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="93f1f-128">Number of unknown device count.</span></span>|
|<span data-ttu-id="93f1f-129">андроиддедикатедкаунт</span><span class="sxs-lookup"><span data-stu-id="93f1f-129">androidDedicatedCount</span></span>|<span data-ttu-id="93f1f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-130">Int32</span></span>|<span data-ttu-id="93f1f-131">Количество выделенных устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="93f1f-131">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="93f1f-132">андроиддевицеадминкаунт</span><span class="sxs-lookup"><span data-stu-id="93f1f-132">androidDeviceAdminCount</span></span>|<span data-ttu-id="93f1f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-133">Int32</span></span>|<span data-ttu-id="93f1f-134">Число устройств с Android для администрирования устройств.</span><span class="sxs-lookup"><span data-stu-id="93f1f-134">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="93f1f-135">андроидфуллиманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="93f1f-135">androidFullyManagedCount</span></span>|<span data-ttu-id="93f1f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-136">Int32</span></span>|<span data-ttu-id="93f1f-137">Количество полностью управляемых устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="93f1f-137">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="93f1f-138">андроидворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="93f1f-138">androidWorkProfileCount</span></span>|<span data-ttu-id="93f1f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="93f1f-139">Int32</span></span>|<span data-ttu-id="93f1f-140">Количество устройств с Android в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="93f1f-140">Number of work profile Android devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93f1f-141">Связи</span><span class="sxs-lookup"><span data-stu-id="93f1f-141">Relationships</span></span>
<span data-ttu-id="93f1f-142">Нет</span><span class="sxs-lookup"><span data-stu-id="93f1f-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93f1f-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93f1f-143">JSON Representation</span></span>
<span data-ttu-id="93f1f-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93f1f-144">Here is a JSON representation of the resource.</span></span>
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
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024
}
```



