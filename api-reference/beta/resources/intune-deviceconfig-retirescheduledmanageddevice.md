---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b79f0541450f4d3c00e4f89f02405cd74545b49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955520"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="c10a5-103">Тип ресурса Ретиресчедуледманажеддевице</span><span class="sxs-lookup"><span data-stu-id="c10a5-103">retireScheduledManagedDevice resource type</span></span>

> <span data-ttu-id="c10a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c10a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c10a5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c10a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c10a5-106">ManagedDevices, для которых запланировано снятие с учета</span><span class="sxs-lookup"><span data-stu-id="c10a5-106">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="c10a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c10a5-107">Properties</span></span>
|<span data-ttu-id="c10a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c10a5-108">Property</span></span>|<span data-ttu-id="c10a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c10a5-109">Type</span></span>|<span data-ttu-id="c10a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c10a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c10a5-111">id</span><span class="sxs-lookup"><span data-stu-id="c10a5-111">id</span></span>|<span data-ttu-id="c10a5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c10a5-112">String</span></span>|<span data-ttu-id="c10a5-113">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c10a5-113">Key of the entity.</span></span>|
|<span data-ttu-id="c10a5-114">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="c10a5-114">managedDeviceId</span></span>|<span data-ttu-id="c10a5-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c10a5-115">String</span></span>|<span data-ttu-id="c10a5-116">Управляемый DeviceId</span><span class="sxs-lookup"><span data-stu-id="c10a5-116">Managed DeviceId</span></span>|
|<span data-ttu-id="c10a5-117">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c10a5-117">managedDeviceName</span></span>|<span data-ttu-id="c10a5-118">String</span><span class="sxs-lookup"><span data-stu-id="c10a5-118">String</span></span>|<span data-ttu-id="c10a5-119">Управляемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="c10a5-119">Managed Device Name</span></span>|
|<span data-ttu-id="c10a5-120">deviceType</span><span class="sxs-lookup"><span data-stu-id="c10a5-120">deviceType</span></span>|[<span data-ttu-id="c10a5-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="c10a5-121">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c10a5-122">Тип устройства управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="c10a5-122">Managed Device Device Type.</span></span> <span data-ttu-id="c10a5-123">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="c10a5-123">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c10a5-124">complianceState</span><span class="sxs-lookup"><span data-stu-id="c10a5-124">complianceState</span></span>|[<span data-ttu-id="c10a5-125">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="c10a5-125">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c10a5-126">Управляемое устройство Комплианцестатус.</span><span class="sxs-lookup"><span data-stu-id="c10a5-126">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="c10a5-127">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c10a5-127">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c10a5-128">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="c10a5-128">retireAfterDateTime</span></span>|<span data-ttu-id="c10a5-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c10a5-129">DateTimeOffset</span></span>|<span data-ttu-id="c10a5-130">Прекращение использования управляемого устройства после даты и времени</span><span class="sxs-lookup"><span data-stu-id="c10a5-130">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="c10a5-131">managementAgent</span><span class="sxs-lookup"><span data-stu-id="c10a5-131">managementAgent</span></span>|[<span data-ttu-id="c10a5-132">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="c10a5-132">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="c10a5-133">Управляемое устройство Манажементаженттипе.</span><span class="sxs-lookup"><span data-stu-id="c10a5-133">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="c10a5-134">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span><span class="sxs-lookup"><span data-stu-id="c10a5-134">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="c10a5-135">ownerType</span><span class="sxs-lookup"><span data-stu-id="c10a5-135">ownerType</span></span>|[<span data-ttu-id="c10a5-136">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="c10a5-136">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="c10a5-137">Управляемое устройство Манажеддевицеовнертипе.</span><span class="sxs-lookup"><span data-stu-id="c10a5-137">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="c10a5-138">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="c10a5-138">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="c10a5-139">девицекомплианцеполицинаме</span><span class="sxs-lookup"><span data-stu-id="c10a5-139">deviceCompliancePolicyName</span></span>|<span data-ttu-id="c10a5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c10a5-140">String</span></span>|<span data-ttu-id="c10a5-141">Имя политики соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="c10a5-141">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="c10a5-142">девицекомплианцеполициид</span><span class="sxs-lookup"><span data-stu-id="c10a5-142">deviceCompliancePolicyId</span></span>|<span data-ttu-id="c10a5-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c10a5-143">String</span></span>|<span data-ttu-id="c10a5-144">Соответствие требованиям устройств Полициид</span><span class="sxs-lookup"><span data-stu-id="c10a5-144">Device Compliance PolicyId</span></span>|

## <a name="relationships"></a><span data-ttu-id="c10a5-145">Связи</span><span class="sxs-lookup"><span data-stu-id="c10a5-145">Relationships</span></span>
<span data-ttu-id="c10a5-146">Нет</span><span class="sxs-lookup"><span data-stu-id="c10a5-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c10a5-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c10a5-147">JSON Representation</span></span>
<span data-ttu-id="c10a5-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c10a5-148">Here is a JSON representation of the resource.</span></span>
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



