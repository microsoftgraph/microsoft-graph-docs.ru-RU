---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9557780ffbf2d82edecdcdcaa747fe3cbd1bf8c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787602"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="67351-103">Тип ресурса Ретиресчедуледманажеддевице</span><span class="sxs-lookup"><span data-stu-id="67351-103">retireScheduledManagedDevice resource type</span></span>

> <span data-ttu-id="67351-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67351-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67351-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67351-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67351-106">ManagedDevices, для которых запланировано снятие с учета</span><span class="sxs-lookup"><span data-stu-id="67351-106">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="67351-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67351-107">Properties</span></span>
|<span data-ttu-id="67351-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="67351-108">Property</span></span>|<span data-ttu-id="67351-109">Тип</span><span class="sxs-lookup"><span data-stu-id="67351-109">Type</span></span>|<span data-ttu-id="67351-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67351-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67351-111">id</span><span class="sxs-lookup"><span data-stu-id="67351-111">id</span></span>|<span data-ttu-id="67351-112">String</span><span class="sxs-lookup"><span data-stu-id="67351-112">String</span></span>|<span data-ttu-id="67351-113">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67351-113">Key of the entity.</span></span>|
|<span data-ttu-id="67351-114">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="67351-114">managedDeviceId</span></span>|<span data-ttu-id="67351-115">String</span><span class="sxs-lookup"><span data-stu-id="67351-115">String</span></span>|<span data-ttu-id="67351-116">Управляемый DeviceId</span><span class="sxs-lookup"><span data-stu-id="67351-116">Managed DeviceId</span></span>|
|<span data-ttu-id="67351-117">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="67351-117">managedDeviceName</span></span>|<span data-ttu-id="67351-118">String</span><span class="sxs-lookup"><span data-stu-id="67351-118">String</span></span>|<span data-ttu-id="67351-119">Управляемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="67351-119">Managed Device Name</span></span>|
|<span data-ttu-id="67351-120">deviceType</span><span class="sxs-lookup"><span data-stu-id="67351-120">deviceType</span></span>|[<span data-ttu-id="67351-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="67351-121">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="67351-122">Тип устройства управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="67351-122">Managed Device Device Type.</span></span> <span data-ttu-id="67351-123">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="67351-123">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="67351-124">complianceState</span><span class="sxs-lookup"><span data-stu-id="67351-124">complianceState</span></span>|[<span data-ttu-id="67351-125">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="67351-125">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="67351-126">Управляемое устройство Комплианцестатус.</span><span class="sxs-lookup"><span data-stu-id="67351-126">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="67351-127">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="67351-127">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="67351-128">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="67351-128">retireAfterDateTime</span></span>|<span data-ttu-id="67351-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67351-129">DateTimeOffset</span></span>|<span data-ttu-id="67351-130">Прекращение использования управляемого устройства после даты и времени</span><span class="sxs-lookup"><span data-stu-id="67351-130">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="67351-131">managementAgent</span><span class="sxs-lookup"><span data-stu-id="67351-131">managementAgent</span></span>|[<span data-ttu-id="67351-132">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="67351-132">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="67351-133">Управляемое устройство Манажементаженттипе.</span><span class="sxs-lookup"><span data-stu-id="67351-133">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="67351-134">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="67351-134">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="67351-135">ownerType</span><span class="sxs-lookup"><span data-stu-id="67351-135">ownerType</span></span>|[<span data-ttu-id="67351-136">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="67351-136">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="67351-137">Управляемое устройство Манажеддевицеовнертипе.</span><span class="sxs-lookup"><span data-stu-id="67351-137">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="67351-138">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="67351-138">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="67351-139">девицекомплианцеполицинаме</span><span class="sxs-lookup"><span data-stu-id="67351-139">deviceCompliancePolicyName</span></span>|<span data-ttu-id="67351-140">String</span><span class="sxs-lookup"><span data-stu-id="67351-140">String</span></span>|<span data-ttu-id="67351-141">Имя политики соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="67351-141">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="67351-142">девицекомплианцеполициид</span><span class="sxs-lookup"><span data-stu-id="67351-142">deviceCompliancePolicyId</span></span>|<span data-ttu-id="67351-143">String</span><span class="sxs-lookup"><span data-stu-id="67351-143">String</span></span>|<span data-ttu-id="67351-144">Соответствие требованиям устройств Полициид</span><span class="sxs-lookup"><span data-stu-id="67351-144">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="67351-145">Связи</span><span class="sxs-lookup"><span data-stu-id="67351-145">Relationships</span></span>
<span data-ttu-id="67351-146">Нет</span><span class="sxs-lookup"><span data-stu-id="67351-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67351-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67351-147">JSON Representation</span></span>
<span data-ttu-id="67351-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67351-148">Here is a JSON representation of the resource.</span></span>
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



