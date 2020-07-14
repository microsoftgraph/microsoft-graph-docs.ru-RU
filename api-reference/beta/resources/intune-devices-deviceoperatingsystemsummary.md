---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b1a49496357a3688bd9f484d8759fdd0c2140eb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122632"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="a0b91-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a0b91-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="a0b91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0b91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0b91-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0b91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0b91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0b91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0b91-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="a0b91-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="a0b91-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0b91-108">Properties</span></span>
|<span data-ttu-id="a0b91-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0b91-109">Property</span></span>|<span data-ttu-id="a0b91-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a0b91-110">Type</span></span>|<span data-ttu-id="a0b91-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a0b91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0b91-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-112">androidCount</span></span>|<span data-ttu-id="a0b91-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-113">Int32</span></span>|<span data-ttu-id="a0b91-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a0b91-114">Number of android device count.</span></span>|
|<span data-ttu-id="a0b91-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-115">iosCount</span></span>|<span data-ttu-id="a0b91-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-116">Int32</span></span>|<span data-ttu-id="a0b91-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="a0b91-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="a0b91-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-118">macOSCount</span></span>|<span data-ttu-id="a0b91-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-119">Int32</span></span>|<span data-ttu-id="a0b91-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="a0b91-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="a0b91-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-121">windowsMobileCount</span></span>|<span data-ttu-id="a0b91-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-122">Int32</span></span>|<span data-ttu-id="a0b91-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a0b91-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="a0b91-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-124">windowsCount</span></span>|<span data-ttu-id="a0b91-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-125">Int32</span></span>|<span data-ttu-id="a0b91-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a0b91-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="a0b91-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a0b91-127">unknownCount</span></span>|<span data-ttu-id="a0b91-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-128">Int32</span></span>|<span data-ttu-id="a0b91-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a0b91-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="a0b91-130">андроиддедикатедкаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-130">androidDedicatedCount</span></span>|<span data-ttu-id="a0b91-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-131">Int32</span></span>|<span data-ttu-id="a0b91-132">Количество выделенных устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a0b91-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="a0b91-133">андроиддевицеадминкаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="a0b91-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-134">Int32</span></span>|<span data-ttu-id="a0b91-135">Число устройств с Android для администрирования устройств.</span><span class="sxs-lookup"><span data-stu-id="a0b91-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="a0b91-136">андроидфуллиманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-136">androidFullyManagedCount</span></span>|<span data-ttu-id="a0b91-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-137">Int32</span></span>|<span data-ttu-id="a0b91-138">Количество полностью управляемых устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a0b91-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="a0b91-139">андроидворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-139">androidWorkProfileCount</span></span>|<span data-ttu-id="a0b91-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-140">Int32</span></span>|<span data-ttu-id="a0b91-141">Количество устройств с Android в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="a0b91-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="a0b91-142">андроидкорпоратеворкпрофилекаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="a0b91-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-143">Int32</span></span>|<span data-ttu-id="a0b91-144">Количество устройств с Android для корпоративных профилей рабочих профилей.</span><span class="sxs-lookup"><span data-stu-id="a0b91-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="a0b91-145">Также называется корпоративным владельцем.</span><span class="sxs-lookup"><span data-stu-id="a0b91-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="a0b91-146">Допустимые значения: от 1 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a0b91-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="a0b91-147">конфигмгрдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a0b91-147">configMgrDeviceCount</span></span>|<span data-ttu-id="a0b91-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b91-148">Int32</span></span>|<span data-ttu-id="a0b91-149">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="a0b91-149">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0b91-150">Связи</span><span class="sxs-lookup"><span data-stu-id="a0b91-150">Relationships</span></span>
<span data-ttu-id="a0b91-151">Нет</span><span class="sxs-lookup"><span data-stu-id="a0b91-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0b91-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0b91-152">JSON Representation</span></span>
<span data-ttu-id="a0b91-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0b91-153">Here is a JSON representation of the resource.</span></span>
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
  "configMgrDeviceCount": 1024
}
```



