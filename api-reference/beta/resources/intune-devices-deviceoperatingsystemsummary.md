---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a88a86a420aa10b32f44e44bc25276040fc9d99c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784149"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="34405-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="34405-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="34405-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34405-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34405-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34405-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34405-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="34405-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="34405-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="34405-107">Properties</span></span>
|<span data-ttu-id="34405-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="34405-108">Property</span></span>|<span data-ttu-id="34405-109">Тип</span><span class="sxs-lookup"><span data-stu-id="34405-109">Type</span></span>|<span data-ttu-id="34405-110">Описание</span><span class="sxs-lookup"><span data-stu-id="34405-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34405-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="34405-111">androidCount</span></span>|<span data-ttu-id="34405-112">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-112">Int32</span></span>|<span data-ttu-id="34405-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="34405-113">Number of android device count.</span></span>|
|<span data-ttu-id="34405-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="34405-114">iosCount</span></span>|<span data-ttu-id="34405-115">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-115">Int32</span></span>|<span data-ttu-id="34405-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="34405-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="34405-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="34405-117">macOSCount</span></span>|<span data-ttu-id="34405-118">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-118">Int32</span></span>|<span data-ttu-id="34405-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="34405-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="34405-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="34405-120">windowsMobileCount</span></span>|<span data-ttu-id="34405-121">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-121">Int32</span></span>|<span data-ttu-id="34405-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="34405-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="34405-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="34405-123">windowsCount</span></span>|<span data-ttu-id="34405-124">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-124">Int32</span></span>|<span data-ttu-id="34405-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="34405-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="34405-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="34405-126">unknownCount</span></span>|<span data-ttu-id="34405-127">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-127">Int32</span></span>|<span data-ttu-id="34405-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="34405-128">Number of unknown device count.</span></span>|
|<span data-ttu-id="34405-129">андроиддедикатедкаунт</span><span class="sxs-lookup"><span data-stu-id="34405-129">androidDedicatedCount</span></span>|<span data-ttu-id="34405-130">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-130">Int32</span></span>|<span data-ttu-id="34405-131">Количество выделенных устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="34405-131">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="34405-132">андроиддевицеадминкаунт</span><span class="sxs-lookup"><span data-stu-id="34405-132">androidDeviceAdminCount</span></span>|<span data-ttu-id="34405-133">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-133">Int32</span></span>|<span data-ttu-id="34405-134">Число устройств с Android для администрирования устройств.</span><span class="sxs-lookup"><span data-stu-id="34405-134">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="34405-135">андроидфуллиманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="34405-135">androidFullyManagedCount</span></span>|<span data-ttu-id="34405-136">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-136">Int32</span></span>|<span data-ttu-id="34405-137">Количество полностью управляемых устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="34405-137">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="34405-138">андроидворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="34405-138">androidWorkProfileCount</span></span>|<span data-ttu-id="34405-139">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-139">Int32</span></span>|<span data-ttu-id="34405-140">Количество устройств с Android в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="34405-140">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="34405-141">конфигмгрдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="34405-141">configMgrDeviceCount</span></span>|<span data-ttu-id="34405-142">Int32</span><span class="sxs-lookup"><span data-stu-id="34405-142">Int32</span></span>|<span data-ttu-id="34405-143">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="34405-143">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34405-144">Связи</span><span class="sxs-lookup"><span data-stu-id="34405-144">Relationships</span></span>
<span data-ttu-id="34405-145">Нет</span><span class="sxs-lookup"><span data-stu-id="34405-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34405-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34405-146">JSON Representation</span></span>
<span data-ttu-id="34405-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34405-147">Here is a JSON representation of the resource.</span></span>
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
  "androidWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024
}
```



