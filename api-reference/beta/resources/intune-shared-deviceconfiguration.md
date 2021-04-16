---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9f6fb0760457262158110bc7c296feeefa72e26
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867289"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="670f2-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="670f2-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="670f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="670f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="670f2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="670f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="670f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="670f2-107">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="670f2-107">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="670f2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="670f2-108">Methods</span></span>
|<span data-ttu-id="670f2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="670f2-109">Method</span></span>|<span data-ttu-id="670f2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="670f2-110">Return Type</span></span>|<span data-ttu-id="670f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="670f2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="670f2-112">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="670f2-112">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="670f2-113">Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-113">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="670f2-114">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-114">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="670f2-115">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="670f2-115">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="670f2-116">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="670f2-116">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="670f2-117">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-117">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="670f2-118">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="670f2-118">**Device configuration**</span></span>|
|[<span data-ttu-id="670f2-119">Действие assign</span><span class="sxs-lookup"><span data-stu-id="670f2-119">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="670f2-120">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-120">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="670f2-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="670f2-121">Not yet documented</span></span>|
|[<span data-ttu-id="670f2-122">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="670f2-122">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="670f2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="670f2-123">None</span></span>|<span data-ttu-id="670f2-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="670f2-124">Not yet documented</span></span>|
|[<span data-ttu-id="670f2-125">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="670f2-125">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="670f2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="670f2-126">None</span></span>|<span data-ttu-id="670f2-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="670f2-127">Not yet documented</span></span>|
|[<span data-ttu-id="670f2-128">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="670f2-128">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="670f2-129">[коллекция deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-129">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="670f2-130">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="670f2-130">Not yet documented</span></span>|
|<span data-ttu-id="670f2-131">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="670f2-131">**Policy Set**</span></span>|
|[<span data-ttu-id="670f2-132">действие hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="670f2-132">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="670f2-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="670f2-133">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="670f2-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="670f2-134">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="670f2-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="670f2-135">Properties</span></span>
|<span data-ttu-id="670f2-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="670f2-136">Property</span></span>|<span data-ttu-id="670f2-137">Тип</span><span class="sxs-lookup"><span data-stu-id="670f2-137">Type</span></span>|<span data-ttu-id="670f2-138">Описание</span><span class="sxs-lookup"><span data-stu-id="670f2-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670f2-139">id</span><span class="sxs-lookup"><span data-stu-id="670f2-139">id</span></span>|<span data-ttu-id="670f2-140">String</span><span class="sxs-lookup"><span data-stu-id="670f2-140">String</span></span>|<span data-ttu-id="670f2-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="670f2-141">Key of the entity.</span></span>|
|<span data-ttu-id="670f2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="670f2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="670f2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="670f2-143">DateTimeOffset</span></span>|<span data-ttu-id="670f2-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="670f2-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="670f2-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="670f2-145">roleScopeTagIds</span></span>|<span data-ttu-id="670f2-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="670f2-146">String collection</span></span>|<span data-ttu-id="670f2-147">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="670f2-147">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="670f2-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="670f2-148">supportsScopeTags</span></span>|<span data-ttu-id="670f2-149">Логический</span><span class="sxs-lookup"><span data-stu-id="670f2-149">Boolean</span></span>|<span data-ttu-id="670f2-150">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="670f2-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="670f2-151">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="670f2-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="670f2-152">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="670f2-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="670f2-153">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="670f2-153">This property is read-only.</span></span>|
|<span data-ttu-id="670f2-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="670f2-154">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="670f2-155">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="670f2-155">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="670f2-156">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="670f2-156">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="670f2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="670f2-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="670f2-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="670f2-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="670f2-159">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="670f2-159">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="670f2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="670f2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="670f2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="670f2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="670f2-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="670f2-162">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="670f2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="670f2-163">createdDateTime</span></span>|<span data-ttu-id="670f2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="670f2-164">DateTimeOffset</span></span>|<span data-ttu-id="670f2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="670f2-165">DateTime the object was created.</span></span>|
|<span data-ttu-id="670f2-166">description</span><span class="sxs-lookup"><span data-stu-id="670f2-166">description</span></span>|<span data-ttu-id="670f2-167">String</span><span class="sxs-lookup"><span data-stu-id="670f2-167">String</span></span>|<span data-ttu-id="670f2-168">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-168">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="670f2-169">displayName</span><span class="sxs-lookup"><span data-stu-id="670f2-169">displayName</span></span>|<span data-ttu-id="670f2-170">String</span><span class="sxs-lookup"><span data-stu-id="670f2-170">String</span></span>|<span data-ttu-id="670f2-171">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-171">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="670f2-172">version</span><span class="sxs-lookup"><span data-stu-id="670f2-172">version</span></span>|<span data-ttu-id="670f2-173">Int32</span><span class="sxs-lookup"><span data-stu-id="670f2-173">Int32</span></span>|<span data-ttu-id="670f2-174">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-174">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="670f2-175">Связи</span><span class="sxs-lookup"><span data-stu-id="670f2-175">Relationships</span></span>
|<span data-ttu-id="670f2-176">Связь</span><span class="sxs-lookup"><span data-stu-id="670f2-176">Relationship</span></span>|<span data-ttu-id="670f2-177">Тип</span><span class="sxs-lookup"><span data-stu-id="670f2-177">Type</span></span>|<span data-ttu-id="670f2-178">Описание</span><span class="sxs-lookup"><span data-stu-id="670f2-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670f2-179">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="670f2-179">**Device configuration**</span></span>|
|<span data-ttu-id="670f2-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="670f2-180">groupAssignments</span></span>|<span data-ttu-id="670f2-181">[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="670f2-182">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-182">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="670f2-183">assignments</span><span class="sxs-lookup"><span data-stu-id="670f2-183">assignments</span></span>|<span data-ttu-id="670f2-184">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-184">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="670f2-185">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-185">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="670f2-186">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="670f2-186">deviceStatuses</span></span>|<span data-ttu-id="670f2-187">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-187">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="670f2-188">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="670f2-188">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="670f2-189">userStatuses</span><span class="sxs-lookup"><span data-stu-id="670f2-189">userStatuses</span></span>|<span data-ttu-id="670f2-190">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-190">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="670f2-191">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="670f2-191">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="670f2-192">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="670f2-192">deviceStatusOverview</span></span>|[<span data-ttu-id="670f2-193">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="670f2-193">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="670f2-194">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="670f2-194">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="670f2-195">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="670f2-195">userStatusOverview</span></span>|[<span data-ttu-id="670f2-196">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="670f2-196">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="670f2-197">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="670f2-197">Device Configuration users status overview</span></span>|
|<span data-ttu-id="670f2-198">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="670f2-198">deviceSettingStateSummaries</span></span>|<span data-ttu-id="670f2-199">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="670f2-199">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="670f2-200">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="670f2-200">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="670f2-201">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="670f2-201">JSON Representation</span></span>
<span data-ttu-id="670f2-202">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670f2-202">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```




