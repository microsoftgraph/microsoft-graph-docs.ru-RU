---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c15adc462742adb734a503f55dc69af48bf0f82
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470742"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="9c854-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9c854-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="9c854-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c854-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c854-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c854-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="9c854-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="9c854-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c854-108">Properties</span></span>
|<span data-ttu-id="9c854-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c854-109">Property</span></span>|<span data-ttu-id="9c854-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9c854-110">Type</span></span>|<span data-ttu-id="9c854-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9c854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c854-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="9c854-112">androidCount</span></span>|<span data-ttu-id="9c854-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-113">Int32</span></span>|<span data-ttu-id="9c854-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="9c854-114">Number of android device count.</span></span>|
|<span data-ttu-id="9c854-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="9c854-115">iosCount</span></span>|<span data-ttu-id="9c854-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-116">Int32</span></span>|<span data-ttu-id="9c854-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="9c854-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="9c854-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="9c854-118">macOSCount</span></span>|<span data-ttu-id="9c854-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-119">Int32</span></span>|<span data-ttu-id="9c854-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="9c854-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="9c854-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="9c854-121">windowsMobileCount</span></span>|<span data-ttu-id="9c854-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-122">Int32</span></span>|<span data-ttu-id="9c854-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="9c854-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="9c854-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="9c854-124">windowsCount</span></span>|<span data-ttu-id="9c854-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-125">Int32</span></span>|<span data-ttu-id="9c854-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="9c854-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="9c854-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="9c854-127">unknownCount</span></span>|<span data-ttu-id="9c854-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-128">Int32</span></span>|<span data-ttu-id="9c854-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="9c854-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="9c854-130">андроиддедикатедкаунт</span><span class="sxs-lookup"><span data-stu-id="9c854-130">androidDedicatedCount</span></span>|<span data-ttu-id="9c854-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-131">Int32</span></span>|<span data-ttu-id="9c854-132">Количество выделенных устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="9c854-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="9c854-133">андроиддевицеадминкаунт</span><span class="sxs-lookup"><span data-stu-id="9c854-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="9c854-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-134">Int32</span></span>|<span data-ttu-id="9c854-135">Число устройств с Android для администрирования устройств.</span><span class="sxs-lookup"><span data-stu-id="9c854-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="9c854-136">андроидфуллиманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="9c854-136">androidFullyManagedCount</span></span>|<span data-ttu-id="9c854-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-137">Int32</span></span>|<span data-ttu-id="9c854-138">Количество полностью управляемых устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="9c854-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="9c854-139">андроидворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="9c854-139">androidWorkProfileCount</span></span>|<span data-ttu-id="9c854-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-140">Int32</span></span>|<span data-ttu-id="9c854-141">Количество устройств с Android в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="9c854-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="9c854-142">конфигмгрдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9c854-142">configMgrDeviceCount</span></span>|<span data-ttu-id="9c854-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9c854-143">Int32</span></span>|<span data-ttu-id="9c854-144">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="9c854-144">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c854-145">Связи</span><span class="sxs-lookup"><span data-stu-id="9c854-145">Relationships</span></span>
<span data-ttu-id="9c854-146">Нет</span><span class="sxs-lookup"><span data-stu-id="9c854-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c854-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c854-147">JSON Representation</span></span>
<span data-ttu-id="9c854-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c854-148">Here is a JSON representation of the resource.</span></span>
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



