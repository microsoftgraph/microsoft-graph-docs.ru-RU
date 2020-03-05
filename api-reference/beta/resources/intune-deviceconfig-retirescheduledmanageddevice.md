---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 230d688429bb98361c04ad3d28789e0e886361fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529446"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="e06c4-103">Тип ресурса Ретиресчедуледманажеддевице</span><span class="sxs-lookup"><span data-stu-id="e06c4-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="e06c4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e06c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e06c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e06c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e06c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06c4-107">ManagedDevices, для которых запланировано снятие с учета</span><span class="sxs-lookup"><span data-stu-id="e06c4-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="e06c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e06c4-108">Properties</span></span>
|<span data-ttu-id="e06c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e06c4-109">Property</span></span>|<span data-ttu-id="e06c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e06c4-110">Type</span></span>|<span data-ttu-id="e06c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e06c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06c4-112">id</span><span class="sxs-lookup"><span data-stu-id="e06c4-112">id</span></span>|<span data-ttu-id="e06c4-113">String</span><span class="sxs-lookup"><span data-stu-id="e06c4-113">String</span></span>|<span data-ttu-id="e06c4-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e06c4-114">Key of the entity.</span></span>|
|<span data-ttu-id="e06c4-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="e06c4-115">managedDeviceId</span></span>|<span data-ttu-id="e06c4-116">String</span><span class="sxs-lookup"><span data-stu-id="e06c4-116">String</span></span>|<span data-ttu-id="e06c4-117">Управляемый DeviceId</span><span class="sxs-lookup"><span data-stu-id="e06c4-117">Managed DeviceId</span></span>|
|<span data-ttu-id="e06c4-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="e06c4-118">managedDeviceName</span></span>|<span data-ttu-id="e06c4-119">String</span><span class="sxs-lookup"><span data-stu-id="e06c4-119">String</span></span>|<span data-ttu-id="e06c4-120">Управляемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="e06c4-120">Managed Device Name</span></span>|
|<span data-ttu-id="e06c4-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="e06c4-121">deviceType</span></span>|[<span data-ttu-id="e06c4-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="e06c4-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e06c4-123">Тип устройства управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="e06c4-123">Managed Device Device Type.</span></span> <span data-ttu-id="e06c4-124">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="e06c4-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e06c4-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="e06c4-125">complianceState</span></span>|[<span data-ttu-id="e06c4-126">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e06c4-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e06c4-127">Управляемое устройство Комплианцестатус.</span><span class="sxs-lookup"><span data-stu-id="e06c4-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="e06c4-128">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e06c4-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e06c4-129">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="e06c4-129">retireAfterDateTime</span></span>|<span data-ttu-id="e06c4-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e06c4-130">DateTimeOffset</span></span>|<span data-ttu-id="e06c4-131">Прекращение использования управляемого устройства после даты и времени</span><span class="sxs-lookup"><span data-stu-id="e06c4-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="e06c4-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="e06c4-132">managementAgent</span></span>|[<span data-ttu-id="e06c4-133">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="e06c4-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="e06c4-134">Управляемое устройство Манажементаженттипе.</span><span class="sxs-lookup"><span data-stu-id="e06c4-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="e06c4-135">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="e06c4-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="e06c4-136">ownerType</span><span class="sxs-lookup"><span data-stu-id="e06c4-136">ownerType</span></span>|[<span data-ttu-id="e06c4-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="e06c4-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="e06c4-138">Управляемое устройство Манажеддевицеовнертипе.</span><span class="sxs-lookup"><span data-stu-id="e06c4-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="e06c4-139">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="e06c4-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="e06c4-140">девицекомплианцеполицинаме</span><span class="sxs-lookup"><span data-stu-id="e06c4-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="e06c4-141">String</span><span class="sxs-lookup"><span data-stu-id="e06c4-141">String</span></span>|<span data-ttu-id="e06c4-142">Имя политики соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="e06c4-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="e06c4-143">девицекомплианцеполициид</span><span class="sxs-lookup"><span data-stu-id="e06c4-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="e06c4-144">String</span><span class="sxs-lookup"><span data-stu-id="e06c4-144">String</span></span>|<span data-ttu-id="e06c4-145">Соответствие требованиям устройств Полициид</span><span class="sxs-lookup"><span data-stu-id="e06c4-145">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="e06c4-146">Связи</span><span class="sxs-lookup"><span data-stu-id="e06c4-146">Relationships</span></span>
<span data-ttu-id="e06c4-147">Нет</span><span class="sxs-lookup"><span data-stu-id="e06c4-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e06c4-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e06c4-148">JSON Representation</span></span>
<span data-ttu-id="e06c4-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e06c4-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String"
}
```



