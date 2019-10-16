---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68204c747aa983ed44cf2c30fb056baaa7de7225
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539150"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="11936-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11936-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="11936-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11936-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11936-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11936-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11936-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="11936-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="11936-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11936-107">Methods</span></span>
|<span data-ttu-id="11936-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11936-108">Method</span></span>|<span data-ttu-id="11936-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11936-109">Return Type</span></span>|<span data-ttu-id="11936-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11936-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11936-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11936-111">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="11936-112">Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11936-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="11936-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11936-113">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="11936-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11936-114">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="11936-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="11936-115">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="11936-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11936-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="11936-117">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="11936-117">**Device configuration**</span></span>|
|[<span data-ttu-id="11936-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="11936-118">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="11936-119">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11936-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11936-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11936-120">Not yet documented</span></span>|
|[<span data-ttu-id="11936-121">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="11936-121">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="11936-122">Нет</span><span class="sxs-lookup"><span data-stu-id="11936-122">None</span></span>|<span data-ttu-id="11936-123">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="11936-123">Not yet documented</span></span>|
|[<span data-ttu-id="11936-124">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="11936-124">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="11936-125">Нет</span><span class="sxs-lookup"><span data-stu-id="11936-125">None</span></span>|<span data-ttu-id="11936-126">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="11936-126">Not yet documented</span></span>|
|[<span data-ttu-id="11936-127">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="11936-127">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="11936-128">Коллекция [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="11936-128">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="11936-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="11936-129">Not yet documented</span></span>|
|<span data-ttu-id="11936-130">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="11936-130">**Policy Set**</span></span>|
|[<span data-ttu-id="11936-131">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="11936-131">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="11936-132">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="11936-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="11936-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11936-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="11936-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="11936-134">Properties</span></span>
|<span data-ttu-id="11936-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="11936-135">Property</span></span>|<span data-ttu-id="11936-136">Тип</span><span class="sxs-lookup"><span data-stu-id="11936-136">Type</span></span>|<span data-ttu-id="11936-137">Описание</span><span class="sxs-lookup"><span data-stu-id="11936-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11936-138">id</span><span class="sxs-lookup"><span data-stu-id="11936-138">id</span></span>|<span data-ttu-id="11936-139">String</span><span class="sxs-lookup"><span data-stu-id="11936-139">String</span></span>|<span data-ttu-id="11936-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11936-140">Key of the entity.</span></span>|
|<span data-ttu-id="11936-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11936-141">lastModifiedDateTime</span></span>|<span data-ttu-id="11936-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11936-142">DateTimeOffset</span></span>|<span data-ttu-id="11936-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="11936-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="11936-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11936-144">roleScopeTagIds</span></span>|<span data-ttu-id="11936-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="11936-145">String collection</span></span>|<span data-ttu-id="11936-146">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="11936-146">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="11936-147">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="11936-147">supportsScopeTags</span></span>|<span data-ttu-id="11936-148">Логический</span><span class="sxs-lookup"><span data-stu-id="11936-148">Boolean</span></span>|<span data-ttu-id="11936-149">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="11936-149">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="11936-150">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="11936-150">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="11936-151">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="11936-151">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="11936-152">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11936-152">This property is read-only.</span></span>|
|<span data-ttu-id="11936-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11936-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="11936-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="11936-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="11936-155">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="11936-155">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="11936-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11936-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="11936-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="11936-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="11936-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="11936-158">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="11936-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="11936-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="11936-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="11936-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="11936-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="11936-161">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="11936-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11936-162">createdDateTime</span></span>|<span data-ttu-id="11936-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11936-163">DateTimeOffset</span></span>|<span data-ttu-id="11936-164">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="11936-164">DateTime the object was created.</span></span>|
|<span data-ttu-id="11936-165">description</span><span class="sxs-lookup"><span data-stu-id="11936-165">description</span></span>|<span data-ttu-id="11936-166">String</span><span class="sxs-lookup"><span data-stu-id="11936-166">String</span></span>|<span data-ttu-id="11936-167">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-167">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="11936-168">displayName</span><span class="sxs-lookup"><span data-stu-id="11936-168">displayName</span></span>|<span data-ttu-id="11936-169">Строка</span><span class="sxs-lookup"><span data-stu-id="11936-169">String</span></span>|<span data-ttu-id="11936-170">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-170">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="11936-171">version</span><span class="sxs-lookup"><span data-stu-id="11936-171">version</span></span>|<span data-ttu-id="11936-172">Int32</span><span class="sxs-lookup"><span data-stu-id="11936-172">Int32</span></span>|<span data-ttu-id="11936-173">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-173">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11936-174">Связи</span><span class="sxs-lookup"><span data-stu-id="11936-174">Relationships</span></span>
|<span data-ttu-id="11936-175">Связь</span><span class="sxs-lookup"><span data-stu-id="11936-175">Relationship</span></span>|<span data-ttu-id="11936-176">Тип</span><span class="sxs-lookup"><span data-stu-id="11936-176">Type</span></span>|<span data-ttu-id="11936-177">Описание</span><span class="sxs-lookup"><span data-stu-id="11936-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11936-178">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="11936-178">**Device configuration**</span></span>|
|<span data-ttu-id="11936-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="11936-179">groupAssignments</span></span>|<span data-ttu-id="11936-180">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11936-180">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="11936-181">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-181">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="11936-182">assignments</span><span class="sxs-lookup"><span data-stu-id="11936-182">assignments</span></span>|<span data-ttu-id="11936-183">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11936-183">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="11936-184">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-184">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="11936-185">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="11936-185">deviceStatuses</span></span>|<span data-ttu-id="11936-186">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="11936-186">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="11936-187">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="11936-187">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="11936-188">userStatuses</span><span class="sxs-lookup"><span data-stu-id="11936-188">userStatuses</span></span>|<span data-ttu-id="11936-189">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="11936-189">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="11936-190">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="11936-190">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="11936-191">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="11936-191">deviceStatusOverview</span></span>|[<span data-ttu-id="11936-192">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="11936-192">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="11936-193">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="11936-193">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="11936-194">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="11936-194">userStatusOverview</span></span>|[<span data-ttu-id="11936-195">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="11936-195">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="11936-196">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="11936-196">Device Configuration users status overview</span></span>|
|<span data-ttu-id="11936-197">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="11936-197">deviceSettingStateSummaries</span></span>|<span data-ttu-id="11936-198">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="11936-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="11936-199">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="11936-199">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11936-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11936-200">JSON Representation</span></span>
<span data-ttu-id="11936-201">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11936-201">Here is a JSON representation of the resource.</span></span>
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



