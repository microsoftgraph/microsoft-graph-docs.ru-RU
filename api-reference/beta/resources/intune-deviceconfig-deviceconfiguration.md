---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b9bc0bc5c2c589a1eaf1bceb989c981806d553f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001686"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="173e2-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="173e2-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="173e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="173e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="173e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="173e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="173e2-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="173e2-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="173e2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="173e2-107">Methods</span></span>
|<span data-ttu-id="173e2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="173e2-108">Method</span></span>|<span data-ttu-id="173e2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="173e2-109">Return Type</span></span>|<span data-ttu-id="173e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="173e2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="173e2-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="173e2-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="173e2-112">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="173e2-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="173e2-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="173e2-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="173e2-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="173e2-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="173e2-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="173e2-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="173e2-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="173e2-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="173e2-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="173e2-118">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="173e2-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="173e2-119">Not yet documented</span></span>|
|[<span data-ttu-id="173e2-120">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="173e2-120">windowsPrivacyAccessControls action</span></span>](../api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="173e2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="173e2-121">None</span></span>|<span data-ttu-id="173e2-122">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="173e2-122">Not yet documented</span></span>|
|[<span data-ttu-id="173e2-123">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="173e2-123">assignedAccessMultiModeProfiles action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="173e2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="173e2-124">None</span></span>|<span data-ttu-id="173e2-125">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="173e2-125">Not yet documented</span></span>|
|[<span data-ttu-id="173e2-126">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="173e2-126">getTargetedUsersAndDevices action</span></span>](../api/intune-deviceconfig-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="173e2-127">Коллекция [девицеконфигуратионтаржетедусеранддевице](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-127">[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection</span></span>|<span data-ttu-id="173e2-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="173e2-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="173e2-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="173e2-129">Properties</span></span>
|<span data-ttu-id="173e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="173e2-130">Property</span></span>|<span data-ttu-id="173e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="173e2-131">Type</span></span>|<span data-ttu-id="173e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="173e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173e2-133">id</span><span class="sxs-lookup"><span data-stu-id="173e2-133">id</span></span>|<span data-ttu-id="173e2-134">String</span><span class="sxs-lookup"><span data-stu-id="173e2-134">String</span></span>|<span data-ttu-id="173e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="173e2-135">Key of the entity.</span></span>|
|<span data-ttu-id="173e2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="173e2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="173e2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="173e2-137">DateTimeOffset</span></span>|<span data-ttu-id="173e2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="173e2-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="173e2-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="173e2-139">roleScopeTagIds</span></span>|<span data-ttu-id="173e2-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="173e2-140">String collection</span></span>|<span data-ttu-id="173e2-141">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="173e2-141">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="173e2-142">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="173e2-142">supportsScopeTags</span></span>|<span data-ttu-id="173e2-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="173e2-143">Boolean</span></span>|<span data-ttu-id="173e2-144">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="173e2-144">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="173e2-145">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="173e2-145">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="173e2-146">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="173e2-146">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="173e2-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="173e2-147">This property is read-only.</span></span>|
|<span data-ttu-id="173e2-148">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="173e2-148">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="173e2-149">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="173e2-149">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="173e2-150">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="173e2-150">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="173e2-151">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="173e2-151">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="173e2-152">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="173e2-152">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="173e2-153">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="173e2-153">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="173e2-154">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="173e2-154">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="173e2-155">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="173e2-155">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="173e2-156">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="173e2-156">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="173e2-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="173e2-157">createdDateTime</span></span>|<span data-ttu-id="173e2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="173e2-158">DateTimeOffset</span></span>|<span data-ttu-id="173e2-159">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="173e2-159">DateTime the object was created.</span></span>|
|<span data-ttu-id="173e2-160">description</span><span class="sxs-lookup"><span data-stu-id="173e2-160">description</span></span>|<span data-ttu-id="173e2-161">String</span><span class="sxs-lookup"><span data-stu-id="173e2-161">String</span></span>|<span data-ttu-id="173e2-162">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-162">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="173e2-163">displayName</span><span class="sxs-lookup"><span data-stu-id="173e2-163">displayName</span></span>|<span data-ttu-id="173e2-164">Строка</span><span class="sxs-lookup"><span data-stu-id="173e2-164">String</span></span>|<span data-ttu-id="173e2-165">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-165">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="173e2-166">version</span><span class="sxs-lookup"><span data-stu-id="173e2-166">version</span></span>|<span data-ttu-id="173e2-167">Int32</span><span class="sxs-lookup"><span data-stu-id="173e2-167">Int32</span></span>|<span data-ttu-id="173e2-168">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-168">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="173e2-169">Отношения</span><span class="sxs-lookup"><span data-stu-id="173e2-169">Relationships</span></span>
|<span data-ttu-id="173e2-170">Отношение</span><span class="sxs-lookup"><span data-stu-id="173e2-170">Relationship</span></span>|<span data-ttu-id="173e2-171">Тип</span><span class="sxs-lookup"><span data-stu-id="173e2-171">Type</span></span>|<span data-ttu-id="173e2-172">Описание</span><span class="sxs-lookup"><span data-stu-id="173e2-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173e2-173">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="173e2-173">groupAssignments</span></span>|<span data-ttu-id="173e2-174">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-174">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="173e2-175">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-175">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="173e2-176">assignments</span><span class="sxs-lookup"><span data-stu-id="173e2-176">assignments</span></span>|<span data-ttu-id="173e2-177">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-177">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="173e2-178">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-178">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="173e2-179">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="173e2-179">deviceStatuses</span></span>|<span data-ttu-id="173e2-180">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-180">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="173e2-181">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="173e2-181">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="173e2-182">userStatuses</span><span class="sxs-lookup"><span data-stu-id="173e2-182">userStatuses</span></span>|<span data-ttu-id="173e2-183">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-183">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="173e2-184">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="173e2-184">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="173e2-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="173e2-185">deviceStatusOverview</span></span>|[<span data-ttu-id="173e2-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="173e2-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="173e2-187">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="173e2-187">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="173e2-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="173e2-188">userStatusOverview</span></span>|[<span data-ttu-id="173e2-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="173e2-189">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="173e2-190">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="173e2-190">Device Configuration users status overview</span></span>|
|<span data-ttu-id="173e2-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="173e2-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="173e2-192">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="173e2-192">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="173e2-193">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="173e2-193">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="173e2-194">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="173e2-194">JSON Representation</span></span>
<span data-ttu-id="173e2-195">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="173e2-195">Here is a JSON representation of the resource.</span></span>
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





