---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de94b00a1660dc874e457d20315df2f3b0690164
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444485"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="9f495-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9f495-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="9f495-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f495-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f495-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f495-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f495-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f495-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f495-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="9f495-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="9f495-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f495-108">Properties</span></span>
|<span data-ttu-id="9f495-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f495-109">Property</span></span>|<span data-ttu-id="9f495-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9f495-110">Type</span></span>|<span data-ttu-id="9f495-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f495-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f495-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="9f495-112">androidCount</span></span>|<span data-ttu-id="9f495-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-113">Int32</span></span>|<span data-ttu-id="9f495-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="9f495-114">Number of android device count.</span></span>|
|<span data-ttu-id="9f495-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="9f495-115">iosCount</span></span>|<span data-ttu-id="9f495-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-116">Int32</span></span>|<span data-ttu-id="9f495-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="9f495-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="9f495-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="9f495-118">macOSCount</span></span>|<span data-ttu-id="9f495-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-119">Int32</span></span>|<span data-ttu-id="9f495-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="9f495-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="9f495-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="9f495-121">windowsMobileCount</span></span>|<span data-ttu-id="9f495-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-122">Int32</span></span>|<span data-ttu-id="9f495-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="9f495-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="9f495-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="9f495-124">windowsCount</span></span>|<span data-ttu-id="9f495-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-125">Int32</span></span>|<span data-ttu-id="9f495-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="9f495-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="9f495-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="9f495-127">unknownCount</span></span>|<span data-ttu-id="9f495-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-128">Int32</span></span>|<span data-ttu-id="9f495-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="9f495-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="9f495-130">AndroidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="9f495-130">androidDedicatedCount</span></span>|<span data-ttu-id="9f495-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-131">Int32</span></span>|<span data-ttu-id="9f495-132">Количество выделенных android-устройств.</span><span class="sxs-lookup"><span data-stu-id="9f495-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="9f495-133">AndroidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="9f495-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="9f495-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-134">Int32</span></span>|<span data-ttu-id="9f495-135">Количество устройств администратора устройств Android.</span><span class="sxs-lookup"><span data-stu-id="9f495-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="9f495-136">AndroidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="9f495-136">androidFullyManagedCount</span></span>|<span data-ttu-id="9f495-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-137">Int32</span></span>|<span data-ttu-id="9f495-138">Количество полностью управляемых android-устройств.</span><span class="sxs-lookup"><span data-stu-id="9f495-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="9f495-139">AndroidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="9f495-139">androidWorkProfileCount</span></span>|<span data-ttu-id="9f495-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-140">Int32</span></span>|<span data-ttu-id="9f495-141">Количество устройств Android профиля работы.</span><span class="sxs-lookup"><span data-stu-id="9f495-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="9f495-142">AndroidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="9f495-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="9f495-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-143">Int32</span></span>|<span data-ttu-id="9f495-144">Количество устройств Android корпоративного профиля работы.</span><span class="sxs-lookup"><span data-stu-id="9f495-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="9f495-145">Также известный как корпоративный личный включен (COPE).</span><span class="sxs-lookup"><span data-stu-id="9f495-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="9f495-146">Допустимые значения -1 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f495-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="9f495-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f495-147">configMgrDeviceCount</span></span>|<span data-ttu-id="9f495-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-148">Int32</span></span>|<span data-ttu-id="9f495-149">Количество управляемых устройств ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="9f495-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="9f495-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="9f495-150">aospUserlessCount</span></span>|<span data-ttu-id="9f495-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-151">Int32</span></span>|<span data-ttu-id="9f495-152">Количество устройств без пользователей AOSP для Android.</span><span class="sxs-lookup"><span data-stu-id="9f495-152">Number of AOSP userless Android devices.</span></span> <span data-ttu-id="9f495-153">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f495-153">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="9f495-154">aospUserAssociatedCount</span><span class="sxs-lookup"><span data-stu-id="9f495-154">aospUserAssociatedCount</span></span>|<span data-ttu-id="9f495-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-155">Int32</span></span>|<span data-ttu-id="9f495-156">Количество устройств Android, связанных с пользователем AOSP.</span><span class="sxs-lookup"><span data-stu-id="9f495-156">Number of AOSP user-associated Android devices.</span></span> <span data-ttu-id="9f495-157">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f495-157">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="9f495-158">LinuxCount</span><span class="sxs-lookup"><span data-stu-id="9f495-158">linuxCount</span></span>|<span data-ttu-id="9f495-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9f495-159">Int32</span></span>|<span data-ttu-id="9f495-160">Количество устройств ОС Linux.</span><span class="sxs-lookup"><span data-stu-id="9f495-160">Number of Linux OS devices.</span></span> <span data-ttu-id="9f495-161">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9f495-161">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f495-162">Связи</span><span class="sxs-lookup"><span data-stu-id="9f495-162">Relationships</span></span>
<span data-ttu-id="9f495-163">Нет</span><span class="sxs-lookup"><span data-stu-id="9f495-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f495-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f495-164">JSON Representation</span></span>
<span data-ttu-id="9f495-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f495-165">Here is a JSON representation of the resource.</span></span>
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
  "linuxCount": 1024
}
```




