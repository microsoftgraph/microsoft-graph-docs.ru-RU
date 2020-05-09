---
title: Тип ресурса Ретиресчедуледманажеддевице
description: ManagedDevices, для которых запланировано снятие с учета
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2187035f0f36cc6ae34d706d1bc0054b90584687
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178908"
---
# <a name="retirescheduledmanageddevice-resource-type"></a><span data-ttu-id="8f5ab-103">Тип ресурса Ретиресчедуледманажеддевице</span><span class="sxs-lookup"><span data-stu-id="8f5ab-103">retireScheduledManagedDevice resource type</span></span>

<span data-ttu-id="8f5ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f5ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f5ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f5ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f5ab-107">ManagedDevices, для которых запланировано снятие с учета</span><span class="sxs-lookup"><span data-stu-id="8f5ab-107">ManagedDevices that are scheduled for retire</span></span>

## <a name="properties"></a><span data-ttu-id="8f5ab-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f5ab-108">Properties</span></span>
|<span data-ttu-id="8f5ab-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f5ab-109">Property</span></span>|<span data-ttu-id="8f5ab-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5ab-110">Type</span></span>|<span data-ttu-id="8f5ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f5ab-112">id</span><span class="sxs-lookup"><span data-stu-id="8f5ab-112">id</span></span>|<span data-ttu-id="8f5ab-113">Строка</span><span class="sxs-lookup"><span data-stu-id="8f5ab-113">String</span></span>|<span data-ttu-id="8f5ab-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-114">Key of the entity.</span></span>|
|<span data-ttu-id="8f5ab-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="8f5ab-115">managedDeviceId</span></span>|<span data-ttu-id="8f5ab-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8f5ab-116">String</span></span>|<span data-ttu-id="8f5ab-117">Управляемый DeviceId</span><span class="sxs-lookup"><span data-stu-id="8f5ab-117">Managed DeviceId</span></span>|
|<span data-ttu-id="8f5ab-118">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="8f5ab-118">managedDeviceName</span></span>|<span data-ttu-id="8f5ab-119">String</span><span class="sxs-lookup"><span data-stu-id="8f5ab-119">String</span></span>|<span data-ttu-id="8f5ab-120">Управляемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="8f5ab-120">Managed Device Name</span></span>|
|<span data-ttu-id="8f5ab-121">deviceType</span><span class="sxs-lookup"><span data-stu-id="8f5ab-121">deviceType</span></span>|[<span data-ttu-id="8f5ab-122">deviceType</span><span class="sxs-lookup"><span data-stu-id="8f5ab-122">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="8f5ab-123">Тип устройства управляемого устройства.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-123">Managed Device Device Type.</span></span> <span data-ttu-id="8f5ab-124">Возможные `desktop`значения:, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry` `palm` `unknown`,,,,,,, `iSocConsumer`,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="8f5ab-124">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="8f5ab-125">complianceState</span><span class="sxs-lookup"><span data-stu-id="8f5ab-125">complianceState</span></span>|[<span data-ttu-id="8f5ab-126">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8f5ab-126">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8f5ab-127">Управляемое устройство Комплианцестатус.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-127">Managed Device ComplianceStatus.</span></span> <span data-ttu-id="8f5ab-128">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-128">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8f5ab-129">ретиреафтердатетиме</span><span class="sxs-lookup"><span data-stu-id="8f5ab-129">retireAfterDateTime</span></span>|<span data-ttu-id="8f5ab-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f5ab-130">DateTimeOffset</span></span>|<span data-ttu-id="8f5ab-131">Прекращение использования управляемого устройства после даты и времени</span><span class="sxs-lookup"><span data-stu-id="8f5ab-131">Managed Device Retire After DateTime</span></span>|
|<span data-ttu-id="8f5ab-132">managementAgent</span><span class="sxs-lookup"><span data-stu-id="8f5ab-132">managementAgent</span></span>|[<span data-ttu-id="8f5ab-133">манажементаженттипе</span><span class="sxs-lookup"><span data-stu-id="8f5ab-133">managementAgentType</span></span>](../resources/intune-shared-managementagenttype.md)|<span data-ttu-id="8f5ab-134">Управляемое устройство Манажементаженттипе.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-134">Managed Device ManagementAgentType.</span></span> <span data-ttu-id="8f5ab-135">Возможные значения: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-135">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`.</span></span>|
|<span data-ttu-id="8f5ab-136">ownerType</span><span class="sxs-lookup"><span data-stu-id="8f5ab-136">ownerType</span></span>|[<span data-ttu-id="8f5ab-137">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="8f5ab-137">managedDeviceOwnerType</span></span>](../resources/intune-shared-manageddeviceownertype.md)|<span data-ttu-id="8f5ab-138">Управляемое устройство Манажеддевицеовнертипе.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-138">Managed Device ManagedDeviceOwnerType.</span></span> <span data-ttu-id="8f5ab-139">Возможные значения: `unknown`, `company`, `personal`.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-139">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="8f5ab-140">девицекомплианцеполицинаме</span><span class="sxs-lookup"><span data-stu-id="8f5ab-140">deviceCompliancePolicyName</span></span>|<span data-ttu-id="8f5ab-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8f5ab-141">String</span></span>|<span data-ttu-id="8f5ab-142">Имя политики соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="8f5ab-142">Device Compliance Policy Name</span></span>|
|<span data-ttu-id="8f5ab-143">девицекомплианцеполициид</span><span class="sxs-lookup"><span data-stu-id="8f5ab-143">deviceCompliancePolicyId</span></span>|<span data-ttu-id="8f5ab-144">Строка</span><span class="sxs-lookup"><span data-stu-id="8f5ab-144">String</span></span>|<span data-ttu-id="8f5ab-145">Соответствие требованиям устройств Полициид</span><span class="sxs-lookup"><span data-stu-id="8f5ab-145">Device Compliance PolicyId</span></span>|
|<span data-ttu-id="8f5ab-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f5ab-146">roleScopeTagIds</span></span>|<span data-ttu-id="8f5ab-147">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8f5ab-147">String collection</span></span>|<span data-ttu-id="8f5ab-148">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-148">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f5ab-149">Связи</span><span class="sxs-lookup"><span data-stu-id="8f5ab-149">Relationships</span></span>
<span data-ttu-id="8f5ab-150">Нет</span><span class="sxs-lookup"><span data-stu-id="8f5ab-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f5ab-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f5ab-151">JSON Representation</span></span>
<span data-ttu-id="8f5ab-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f5ab-152">Here is a JSON representation of the resource.</span></span>
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



