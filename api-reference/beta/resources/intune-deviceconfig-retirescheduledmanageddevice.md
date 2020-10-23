---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2939da221a47e878414c5a24f2ed44fdd9c5e238
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729681"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="eff0b-103">Тип ресурса Ретиресчедуледманажеддевице</span><span class="sxs-lookup"><span data-stu-id="eff0b-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="eff0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eff0b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eff0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eff0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eff0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eff0b-107">ManagedDevices, для которых запланировано снятие с учета</span><span class="sxs-lookup"><span data-stu-id="eff0b-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="eff0b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eff0b-108">Properties</span></span>
|<span data-ttu-id="eff0b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eff0b-109">Property</span></span>|<span data-ttu-id="eff0b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eff0b-110">Type</span></span>|<span data-ttu-id="eff0b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eff0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eff0b-112">id</span><span class="sxs-lookup"><span data-stu-id="eff0b-112">id</span></span>|<span data-ttu-id="eff0b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="eff0b-113">String</span></span>|<span data-ttu-id="eff0b-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eff0b-114">Key of the entity.</span></span>|
|<span data-ttu-id="eff0b-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="eff0b-115">managedDeviceId</span></span>|<span data-ttu-id="eff0b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="eff0b-116">String</span></span>|<span data-ttu-id="eff0b-117">Управляемый DeviceId</span><span class="sxs-lookup"><span data-stu-id="eff0b-117">Managed DeviceId</span></span>|
|<span data-ttu-id="eff0b-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="eff0b-118">managedDeviceName</span></span>|<span data-ttu-id="eff0b-119">String</span><span class="sxs-lookup"><span data-stu-id="eff0b-119">String</span></span>|<span data-ttu-id="eff0b-120">Управляемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="eff0b-120">Managed Device Name</span></span>|
|<span data-ttu-id="eff0b-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="eff0b-121">deviceType</span></span>|[<span data-ttu-id="eff0b-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="eff0b-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="eff0b-123">Тип устройства управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="eff0b-123">Managed Device Device Type.</span></span> <span data-ttu-id="eff0b-124">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="eff0b-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="eff0b-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="eff0b-125">complianceState</span></span>|[<span data-ttu-id="eff0b-126">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="eff0b-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="eff0b-127">Управляемое устройство Комплианцестатус.</span><span class="sxs-lookup"><span data-stu-id="eff0b-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="eff0b-128">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="eff0b-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="eff0b-129">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="eff0b-129">retireAfterDateTime</span></span>|<span data-ttu-id="eff0b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eff0b-130">DateTimeOffset</span></span>|<span data-ttu-id="eff0b-131">Прекращение использования управляемого устройства после даты и времени</span><span class="sxs-lookup"><span data-stu-id="eff0b-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="eff0b-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="eff0b-132">managementAgent</span></span>|[<span data-ttu-id="eff0b-133">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="eff0b-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="eff0b-134">Управляемое устройство Манажементаженттипе.</span><span class="sxs-lookup"><span data-stu-id="eff0b-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="eff0b-135">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="eff0b-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="eff0b-136">ownerType</span><span class="sxs-lookup"><span data-stu-id="eff0b-136">ownerType</span></span>|[<span data-ttu-id="eff0b-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="eff0b-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="eff0b-138">Управляемое устройство Манажеддевицеовнертипе.</span><span class="sxs-lookup"><span data-stu-id="eff0b-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="eff0b-139">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="eff0b-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="eff0b-140">девицекомплианцеполицинаме</span><span class="sxs-lookup"><span data-stu-id="eff0b-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="eff0b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="eff0b-141">String</span></span>|<span data-ttu-id="eff0b-142">Имя политики соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="eff0b-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="eff0b-143">девицекомплианцеполициид</span><span class="sxs-lookup"><span data-stu-id="eff0b-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="eff0b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="eff0b-144">String</span></span>|<span data-ttu-id="eff0b-145">Соответствие требованиям устройств Полициид</span><span class="sxs-lookup"><span data-stu-id="eff0b-145">Device Compliance PolicyId</span></span>|
|<span data-ttu-id="eff0b-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eff0b-146">roleScopeTagIds</span></span>|<span data-ttu-id="eff0b-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eff0b-147">String collection</span></span>|<span data-ttu-id="eff0b-148">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="eff0b-148">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eff0b-149">Связи</span><span class="sxs-lookup"><span data-stu-id="eff0b-149">Relationships</span></span>
<span data-ttu-id="eff0b-150">Нет</span><span class="sxs-lookup"><span data-stu-id="eff0b-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eff0b-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eff0b-151">JSON Representation</span></span>
<span data-ttu-id="eff0b-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eff0b-152">Here is a JSON representation of the resource.</span></span>
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
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





