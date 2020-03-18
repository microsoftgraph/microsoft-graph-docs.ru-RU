---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f50fd3038098ebb8381d6872cfa34e86fb8e30e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771210"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="854af-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="854af-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="854af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="854af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="854af-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="854af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="854af-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="854af-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="854af-107">Методы</span><span class="sxs-lookup"><span data-stu-id="854af-107">Methods</span></span>
|<span data-ttu-id="854af-108">Метод</span><span class="sxs-lookup"><span data-stu-id="854af-108">Method</span></span>|<span data-ttu-id="854af-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="854af-109">Return Type</span></span>|<span data-ttu-id="854af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="854af-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="854af-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="854af-111">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="854af-112">Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="854af-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="854af-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="854af-113">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="854af-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="854af-114">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="854af-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="854af-115">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="854af-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="854af-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="854af-117">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="854af-117">**Device configuration**</span></span>|
|[<span data-ttu-id="854af-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="854af-118">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="854af-119">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="854af-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="854af-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="854af-120">Not yet documented</span></span>|
|[<span data-ttu-id="854af-121">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="854af-121">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="854af-122">Нет</span><span class="sxs-lookup"><span data-stu-id="854af-122">None</span></span>|<span data-ttu-id="854af-123">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="854af-123">Not yet documented</span></span>|
|[<span data-ttu-id="854af-124">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="854af-124">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="854af-125">Нет</span><span class="sxs-lookup"><span data-stu-id="854af-125">None</span></span>|<span data-ttu-id="854af-126">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="854af-126">Not yet documented</span></span>|
|[<span data-ttu-id="854af-127">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="854af-127">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="854af-128">Коллекция [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="854af-128">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="854af-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="854af-129">Not yet documented</span></span>|
|<span data-ttu-id="854af-130">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="854af-130">**Policy Set**</span></span>|
|[<span data-ttu-id="854af-131">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="854af-131">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="854af-132">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="854af-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="854af-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="854af-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="854af-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="854af-134">Properties</span></span>
|<span data-ttu-id="854af-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="854af-135">Property</span></span>|<span data-ttu-id="854af-136">Тип</span><span class="sxs-lookup"><span data-stu-id="854af-136">Type</span></span>|<span data-ttu-id="854af-137">Описание</span><span class="sxs-lookup"><span data-stu-id="854af-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854af-138">id</span><span class="sxs-lookup"><span data-stu-id="854af-138">id</span></span>|<span data-ttu-id="854af-139">String</span><span class="sxs-lookup"><span data-stu-id="854af-139">String</span></span>|<span data-ttu-id="854af-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="854af-140">Key of the entity.</span></span>|
|<span data-ttu-id="854af-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="854af-141">lastModifiedDateTime</span></span>|<span data-ttu-id="854af-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="854af-142">DateTimeOffset</span></span>|<span data-ttu-id="854af-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="854af-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="854af-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="854af-144">roleScopeTagIds</span></span>|<span data-ttu-id="854af-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="854af-145">String collection</span></span>|<span data-ttu-id="854af-146">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="854af-146">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="854af-147">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="854af-147">supportsScopeTags</span></span>|<span data-ttu-id="854af-148">Логический</span><span class="sxs-lookup"><span data-stu-id="854af-148">Boolean</span></span>|<span data-ttu-id="854af-149">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="854af-149">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="854af-150">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="854af-150">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="854af-151">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="854af-151">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="854af-152">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="854af-152">This property is read-only.</span></span>|
|<span data-ttu-id="854af-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="854af-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="854af-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="854af-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="854af-155">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="854af-155">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="854af-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="854af-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="854af-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="854af-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="854af-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="854af-158">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="854af-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="854af-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="854af-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="854af-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="854af-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="854af-161">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="854af-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="854af-162">createdDateTime</span></span>|<span data-ttu-id="854af-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="854af-163">DateTimeOffset</span></span>|<span data-ttu-id="854af-164">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="854af-164">DateTime the object was created.</span></span>|
|<span data-ttu-id="854af-165">description</span><span class="sxs-lookup"><span data-stu-id="854af-165">description</span></span>|<span data-ttu-id="854af-166">String</span><span class="sxs-lookup"><span data-stu-id="854af-166">String</span></span>|<span data-ttu-id="854af-167">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-167">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="854af-168">displayName</span><span class="sxs-lookup"><span data-stu-id="854af-168">displayName</span></span>|<span data-ttu-id="854af-169">Строка</span><span class="sxs-lookup"><span data-stu-id="854af-169">String</span></span>|<span data-ttu-id="854af-170">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-170">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="854af-171">version</span><span class="sxs-lookup"><span data-stu-id="854af-171">version</span></span>|<span data-ttu-id="854af-172">Int32</span><span class="sxs-lookup"><span data-stu-id="854af-172">Int32</span></span>|<span data-ttu-id="854af-173">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-173">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="854af-174">Связи</span><span class="sxs-lookup"><span data-stu-id="854af-174">Relationships</span></span>
|<span data-ttu-id="854af-175">Связь</span><span class="sxs-lookup"><span data-stu-id="854af-175">Relationship</span></span>|<span data-ttu-id="854af-176">Тип</span><span class="sxs-lookup"><span data-stu-id="854af-176">Type</span></span>|<span data-ttu-id="854af-177">Описание</span><span class="sxs-lookup"><span data-stu-id="854af-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854af-178">**Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="854af-178">**Device configuration**</span></span>|
|<span data-ttu-id="854af-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="854af-179">groupAssignments</span></span>|<span data-ttu-id="854af-180">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="854af-180">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="854af-181">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-181">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="854af-182">assignments</span><span class="sxs-lookup"><span data-stu-id="854af-182">assignments</span></span>|<span data-ttu-id="854af-183">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="854af-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="854af-184">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-184">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="854af-185">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="854af-185">deviceStatuses</span></span>|<span data-ttu-id="854af-186">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="854af-186">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="854af-187">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="854af-187">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="854af-188">userStatuses</span><span class="sxs-lookup"><span data-stu-id="854af-188">userStatuses</span></span>|<span data-ttu-id="854af-189">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="854af-189">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="854af-190">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="854af-190">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="854af-191">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="854af-191">deviceStatusOverview</span></span>|[<span data-ttu-id="854af-192">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="854af-192">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="854af-193">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="854af-193">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="854af-194">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="854af-194">userStatusOverview</span></span>|[<span data-ttu-id="854af-195">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="854af-195">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="854af-196">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="854af-196">Device Configuration users status overview</span></span>|
|<span data-ttu-id="854af-197">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="854af-197">deviceSettingStateSummaries</span></span>|<span data-ttu-id="854af-198">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="854af-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="854af-199">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="854af-199">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="854af-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="854af-200">JSON Representation</span></span>
<span data-ttu-id="854af-201">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="854af-201">Here is a JSON representation of the resource.</span></span>
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



