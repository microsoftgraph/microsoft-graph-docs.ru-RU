---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba60fc551a3f9de8b795b6521814d7899a1c3706
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755569"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="92411-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="92411-103">deviceManagement resource type</span></span>

<span data-ttu-id="92411-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92411-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92411-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92411-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92411-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="92411-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="92411-107">Методы</span><span class="sxs-lookup"><span data-stu-id="92411-107">Methods</span></span>
|<span data-ttu-id="92411-108">Метод</span><span class="sxs-lookup"><span data-stu-id="92411-108">Method</span></span>|<span data-ttu-id="92411-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92411-109">Return Type</span></span>|<span data-ttu-id="92411-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92411-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92411-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="92411-111">Get deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-get.md)|[<span data-ttu-id="92411-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="92411-112">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="92411-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="92411-113">Read properties and relationships of the [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="92411-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="92411-114">Update deviceManagement</span></span>](../api/intune-deviceconfig-devicemanagement-update.md)|[<span data-ttu-id="92411-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="92411-115">deviceManagement</span></span>](../resources/intune-deviceconfig-devicemanagement.md)|<span data-ttu-id="92411-116">Обновление свойств объекта [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="92411-116">Update the properties of a [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="92411-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="92411-117">Properties</span></span>
|<span data-ttu-id="92411-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="92411-118">Property</span></span>|<span data-ttu-id="92411-119">Тип</span><span class="sxs-lookup"><span data-stu-id="92411-119">Type</span></span>|<span data-ttu-id="92411-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92411-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92411-121">id</span><span class="sxs-lookup"><span data-stu-id="92411-121">id</span></span>|<span data-ttu-id="92411-122">String</span><span class="sxs-lookup"><span data-stu-id="92411-122">String</span></span>|<span data-ttu-id="92411-123">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="92411-123">Unique Identifier</span></span>|
|<span data-ttu-id="92411-124">settings</span><span class="sxs-lookup"><span data-stu-id="92411-124">settings</span></span>|[<span data-ttu-id="92411-125">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="92411-125">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="92411-126">Параметры уровня учетной записи.</span><span class="sxs-lookup"><span data-stu-id="92411-126">Account level settings.</span></span>|
|<span data-ttu-id="92411-127">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="92411-127">intuneAccountId</span></span>|<span data-ttu-id="92411-128">Guid</span><span class="sxs-lookup"><span data-stu-id="92411-128">Guid</span></span>|<span data-ttu-id="92411-129">Id учетной записи Intune для данного клиента</span><span class="sxs-lookup"><span data-stu-id="92411-129">Intune Account Id for given tenant</span></span>|

## <a name="relationships"></a><span data-ttu-id="92411-130">Связи</span><span class="sxs-lookup"><span data-stu-id="92411-130">Relationships</span></span>
|<span data-ttu-id="92411-131">Связь</span><span class="sxs-lookup"><span data-stu-id="92411-131">Relationship</span></span>|<span data-ttu-id="92411-132">Тип</span><span class="sxs-lookup"><span data-stu-id="92411-132">Type</span></span>|<span data-ttu-id="92411-133">Описание</span><span class="sxs-lookup"><span data-stu-id="92411-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92411-134">deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="92411-134">deviceConfigurations</span></span>|<span data-ttu-id="92411-135">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92411-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="92411-136">Конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="92411-136">The device configurations.</span></span>|
|<span data-ttu-id="92411-137">deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="92411-137">deviceCompliancePolicies</span></span>|<span data-ttu-id="92411-138">Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="92411-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="92411-139">Политики соответствия устройств требованиям.</span><span class="sxs-lookup"><span data-stu-id="92411-139">The device compliance policies.</span></span>|
|<span data-ttu-id="92411-140">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="92411-140">softwareUpdateStatusSummary</span></span>|[<span data-ttu-id="92411-141">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="92411-141">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="92411-142">Общие сведения о состоянии обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="92411-142">The software update status summary.</span></span>|
|<span data-ttu-id="92411-143">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="92411-143">deviceCompliancePolicyDeviceStateSummary</span></span>|[<span data-ttu-id="92411-144">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="92411-144">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="92411-145">Общие сведения о состоянии соответствия устройств требованиям для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="92411-145">The device compliance state summary for this account.</span></span>|
|<span data-ttu-id="92411-146">deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="92411-146">deviceCompliancePolicySettingStateSummaries</span></span>|<span data-ttu-id="92411-147">Коллекция [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="92411-147">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) collection</span></span>|<span data-ttu-id="92411-148">Общие сведения о состоянии параметров политики соответствия требованиям для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="92411-148">The summary states of compliance policy settings for this account.</span></span>|
|<span data-ttu-id="92411-149">deviceConfigurationDeviceStateSummaries</span><span class="sxs-lookup"><span data-stu-id="92411-149">deviceConfigurationDeviceStateSummaries</span></span>|[<span data-ttu-id="92411-150">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="92411-150">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="92411-151">Общие сведения о состоянии конфигурации устройства для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="92411-151">The device configuration device state summary for this account.</span></span>|
|<span data-ttu-id="92411-152">iosUpdateStatuses</span><span class="sxs-lookup"><span data-stu-id="92411-152">iosUpdateStatuses</span></span>|<span data-ttu-id="92411-153">Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="92411-153">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) collection</span></span>|<span data-ttu-id="92411-154">Состояния установки обновления программного обеспечения IOS для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="92411-154">The IOS software update installation statuses for this account.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92411-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92411-155">JSON Representation</span></span>
<span data-ttu-id="92411-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92411-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "Guid"
}
```




