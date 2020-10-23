---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74800d0e4b87dbb30d8cc726b0849b12c2061647
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691374"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="1e360-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="1e360-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="1e360-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e360-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e360-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e360-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e360-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e360-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e360-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="1e360-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="1e360-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e360-108">Properties</span></span>
|<span data-ttu-id="1e360-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e360-109">Property</span></span>|<span data-ttu-id="1e360-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1e360-110">Type</span></span>|<span data-ttu-id="1e360-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1e360-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e360-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="1e360-112">androidCount</span></span>|<span data-ttu-id="1e360-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-113">Int32</span></span>|<span data-ttu-id="1e360-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="1e360-114">Number of android device count.</span></span>|
|<span data-ttu-id="1e360-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="1e360-115">iosCount</span></span>|<span data-ttu-id="1e360-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-116">Int32</span></span>|<span data-ttu-id="1e360-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="1e360-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="1e360-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="1e360-118">macOSCount</span></span>|<span data-ttu-id="1e360-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-119">Int32</span></span>|<span data-ttu-id="1e360-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="1e360-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="1e360-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="1e360-121">windowsMobileCount</span></span>|<span data-ttu-id="1e360-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-122">Int32</span></span>|<span data-ttu-id="1e360-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="1e360-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="1e360-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="1e360-124">windowsCount</span></span>|<span data-ttu-id="1e360-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-125">Int32</span></span>|<span data-ttu-id="1e360-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="1e360-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="1e360-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="1e360-127">unknownCount</span></span>|<span data-ttu-id="1e360-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-128">Int32</span></span>|<span data-ttu-id="1e360-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="1e360-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="1e360-130">андроиддедикатедкаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-130">androidDedicatedCount</span></span>|<span data-ttu-id="1e360-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-131">Int32</span></span>|<span data-ttu-id="1e360-132">Количество выделенных устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="1e360-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="1e360-133">андроиддевицеадминкаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="1e360-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-134">Int32</span></span>|<span data-ttu-id="1e360-135">Число устройств с Android для администрирования устройств.</span><span class="sxs-lookup"><span data-stu-id="1e360-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="1e360-136">андроидфуллиманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-136">androidFullyManagedCount</span></span>|<span data-ttu-id="1e360-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-137">Int32</span></span>|<span data-ttu-id="1e360-138">Количество полностью управляемых устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="1e360-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="1e360-139">андроидворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-139">androidWorkProfileCount</span></span>|<span data-ttu-id="1e360-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-140">Int32</span></span>|<span data-ttu-id="1e360-141">Количество устройств с Android в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="1e360-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="1e360-142">андроидкорпоратеворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="1e360-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-143">Int32</span></span>|<span data-ttu-id="1e360-144">Количество устройств с Android для корпоративных профилей рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="1e360-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="1e360-145">Также называется корпоративным владельцем.</span><span class="sxs-lookup"><span data-stu-id="1e360-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="1e360-146">Допустимые значения: от 1 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1e360-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="1e360-147">конфигмгрдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-147">configMgrDeviceCount</span></span>|<span data-ttu-id="1e360-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-148">Int32</span></span>|<span data-ttu-id="1e360-149">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="1e360-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="1e360-150">аоспусерлесскаунт</span><span class="sxs-lookup"><span data-stu-id="1e360-150">aospUserlessCount</span></span>|<span data-ttu-id="1e360-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1e360-151">Int32</span></span>|<span data-ttu-id="1e360-152">Количество выделенных устройств с АОСП для Android.</span><span class="sxs-lookup"><span data-stu-id="1e360-152">Number of AOSP dedicated Android devices.</span></span> <span data-ttu-id="1e360-153">Допустимые значения — от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="1e360-153">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e360-154">Связи</span><span class="sxs-lookup"><span data-stu-id="1e360-154">Relationships</span></span>
<span data-ttu-id="1e360-155">Нет</span><span class="sxs-lookup"><span data-stu-id="1e360-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e360-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e360-156">JSON Representation</span></span>
<span data-ttu-id="1e360-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e360-157">Here is a JSON representation of the resource.</span></span>
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
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024
}
```





