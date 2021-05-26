---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02ab35788ac8628755e0052426c733191fbef2af
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665226"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="a5f94-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a5f94-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="a5f94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5f94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5f94-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5f94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5f94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5f94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f94-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="a5f94-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="a5f94-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5f94-108">Properties</span></span>
|<span data-ttu-id="a5f94-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5f94-109">Property</span></span>|<span data-ttu-id="a5f94-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5f94-110">Type</span></span>|<span data-ttu-id="a5f94-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5f94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f94-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-112">androidCount</span></span>|<span data-ttu-id="a5f94-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-113">Int32</span></span>|<span data-ttu-id="a5f94-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a5f94-114">Number of android device count.</span></span>|
|<span data-ttu-id="a5f94-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-115">iosCount</span></span>|<span data-ttu-id="a5f94-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-116">Int32</span></span>|<span data-ttu-id="a5f94-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="a5f94-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="a5f94-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-118">macOSCount</span></span>|<span data-ttu-id="a5f94-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-119">Int32</span></span>|<span data-ttu-id="a5f94-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="a5f94-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="a5f94-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-121">windowsMobileCount</span></span>|<span data-ttu-id="a5f94-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-122">Int32</span></span>|<span data-ttu-id="a5f94-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a5f94-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="a5f94-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-124">windowsCount</span></span>|<span data-ttu-id="a5f94-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-125">Int32</span></span>|<span data-ttu-id="a5f94-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a5f94-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="a5f94-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-127">unknownCount</span></span>|<span data-ttu-id="a5f94-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-128">Int32</span></span>|<span data-ttu-id="a5f94-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a5f94-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="a5f94-130">AndroidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-130">androidDedicatedCount</span></span>|<span data-ttu-id="a5f94-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-131">Int32</span></span>|<span data-ttu-id="a5f94-132">Количество выделенных android-устройств.</span><span class="sxs-lookup"><span data-stu-id="a5f94-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="a5f94-133">AndroidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="a5f94-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-134">Int32</span></span>|<span data-ttu-id="a5f94-135">Количество устройств администратора устройств Android.</span><span class="sxs-lookup"><span data-stu-id="a5f94-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="a5f94-136">AndroidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-136">androidFullyManagedCount</span></span>|<span data-ttu-id="a5f94-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-137">Int32</span></span>|<span data-ttu-id="a5f94-138">Количество полностью управляемых android-устройств.</span><span class="sxs-lookup"><span data-stu-id="a5f94-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="a5f94-139">AndroidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-139">androidWorkProfileCount</span></span>|<span data-ttu-id="a5f94-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-140">Int32</span></span>|<span data-ttu-id="a5f94-141">Количество устройств Android профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a5f94-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="a5f94-142">AndroidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="a5f94-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-143">Int32</span></span>|<span data-ttu-id="a5f94-144">Количество устройств Android корпоративного профиля работы.</span><span class="sxs-lookup"><span data-stu-id="a5f94-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="a5f94-145">Также известный как корпоративный личный включен (COPE).</span><span class="sxs-lookup"><span data-stu-id="a5f94-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="a5f94-146">Допустимые значения -1 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5f94-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="a5f94-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-147">configMgrDeviceCount</span></span>|<span data-ttu-id="a5f94-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-148">Int32</span></span>|<span data-ttu-id="a5f94-149">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="a5f94-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="a5f94-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-150">aospUserlessCount</span></span>|<span data-ttu-id="a5f94-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-151">Int32</span></span>|<span data-ttu-id="a5f94-152">Количество устройств без пользователей AOSP для Android.</span><span class="sxs-lookup"><span data-stu-id="a5f94-152">Number of AOSP userless Android devices.</span></span> <span data-ttu-id="a5f94-153">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5f94-153">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="a5f94-154">aospUserAssociatedCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-154">aospUserAssociatedCount</span></span>|<span data-ttu-id="a5f94-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-155">Int32</span></span>|<span data-ttu-id="a5f94-156">Количество устройств Android, связанных с пользователем AOSP.</span><span class="sxs-lookup"><span data-stu-id="a5f94-156">Number of AOSP user-associated Android devices.</span></span> <span data-ttu-id="a5f94-157">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5f94-157">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="a5f94-158">LinuxCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-158">linuxCount</span></span>|<span data-ttu-id="a5f94-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-159">Int32</span></span>|<span data-ttu-id="a5f94-160">Количество устройств ОС Linux.</span><span class="sxs-lookup"><span data-stu-id="a5f94-160">Number of Linux OS devices.</span></span> <span data-ttu-id="a5f94-161">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5f94-161">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="a5f94-162">chromeOSCount</span><span class="sxs-lookup"><span data-stu-id="a5f94-162">chromeOSCount</span></span>|<span data-ttu-id="a5f94-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f94-163">Int32</span></span>|<span data-ttu-id="a5f94-164">Количество устройств Chrome OS.</span><span class="sxs-lookup"><span data-stu-id="a5f94-164">Number of Chrome OS devices.</span></span> <span data-ttu-id="a5f94-165">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="a5f94-165">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5f94-166">Связи</span><span class="sxs-lookup"><span data-stu-id="a5f94-166">Relationships</span></span>
<span data-ttu-id="a5f94-167">Нет</span><span class="sxs-lookup"><span data-stu-id="a5f94-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5f94-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5f94-168">JSON Representation</span></span>
<span data-ttu-id="a5f94-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5f94-169">Here is a JSON representation of the resource.</span></span>
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
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024,
  "linuxCount": 1024,
  "chromeOSCount": 1024
}
```




