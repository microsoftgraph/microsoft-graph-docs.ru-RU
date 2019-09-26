---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b595f8fdcc680ff93693f0fcee7f618386aa0740
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201236"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="f710a-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f710a-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="f710a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f710a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f710a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f710a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f710a-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="f710a-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f710a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f710a-107">Methods</span></span>
|<span data-ttu-id="f710a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f710a-108">Method</span></span>|<span data-ttu-id="f710a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f710a-109">Return Type</span></span>|<span data-ttu-id="f710a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f710a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f710a-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f710a-111">List deviceConfigurations</span></span>](../api/intune-shared-deviceconfiguration-list.md)|<span data-ttu-id="f710a-112">Коллекция [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f710a-112">[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="f710a-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f710a-113">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f710a-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f710a-114">Get deviceConfiguration</span></span>](../api/intune-shared-deviceconfiguration-get.md)|[<span data-ttu-id="f710a-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f710a-115">deviceConfiguration</span></span>](../resources/intune-shared-deviceconfiguration.md)|<span data-ttu-id="f710a-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f710a-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>|
|<span data-ttu-id="f710a-117">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="f710a-117">**Device configuration**</span></span>|
|[<span data-ttu-id="f710a-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="f710a-118">assign action</span></span>](../api/intune-shared-deviceconfiguration-assign.md)|<span data-ttu-id="f710a-119">Коллекция deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f710a-119">deviceConfigurationAssignment collection</span></span>|<span data-ttu-id="f710a-120">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f710a-120">Not yet documented</span></span>|
|[<span data-ttu-id="f710a-121">Действие windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="f710a-121">windowsPrivacyAccessControls action</span></span>](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|<span data-ttu-id="f710a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f710a-122">None</span></span>|<span data-ttu-id="f710a-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f710a-123">Not yet documented</span></span>|
|[<span data-ttu-id="f710a-124">Действие assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="f710a-124">assignedAccessMultiModeProfiles action</span></span>](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|<span data-ttu-id="f710a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f710a-125">None</span></span>|<span data-ttu-id="f710a-126">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f710a-126">Not yet documented</span></span>|
|[<span data-ttu-id="f710a-127">Действие getTargetedUsersAndDevices</span><span class="sxs-lookup"><span data-stu-id="f710a-127">getTargetedUsersAndDevices action</span></span>](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|<span data-ttu-id="f710a-128">Коллекция Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="f710a-128">deviceConfigurationTargetedUserAndDevice collection</span></span>|<span data-ttu-id="f710a-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f710a-129">Not yet documented</span></span>|
|<span data-ttu-id="f710a-130">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="f710a-130">**Policy Set**</span></span>|
|[<span data-ttu-id="f710a-131">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="f710a-131">hasPayloadLinks action</span></span>](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|<span data-ttu-id="f710a-132">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="f710a-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="f710a-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f710a-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f710a-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="f710a-134">Properties</span></span>
|<span data-ttu-id="f710a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="f710a-135">Property</span></span>|<span data-ttu-id="f710a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f710a-136">Type</span></span>|<span data-ttu-id="f710a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f710a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f710a-138">id</span><span class="sxs-lookup"><span data-stu-id="f710a-138">id</span></span>|<span data-ttu-id="f710a-139">String</span><span class="sxs-lookup"><span data-stu-id="f710a-139">String</span></span>|<span data-ttu-id="f710a-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f710a-140">Key of the entity.</span></span>|
|<span data-ttu-id="f710a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f710a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f710a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f710a-142">DateTimeOffset</span></span>|<span data-ttu-id="f710a-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f710a-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f710a-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f710a-144">roleScopeTagIds</span></span>|<span data-ttu-id="f710a-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f710a-145">String collection</span></span>|<span data-ttu-id="f710a-146">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f710a-146">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="f710a-147">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f710a-147">supportsScopeTags</span></span>|<span data-ttu-id="f710a-148">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f710a-148">Boolean</span></span>|<span data-ttu-id="f710a-149">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f710a-149">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f710a-150">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f710a-150">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f710a-151">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f710a-151">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f710a-152">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f710a-152">This property is read-only.</span></span>|
|<span data-ttu-id="f710a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f710a-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f710a-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f710a-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f710a-155">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f710a-155">The OS edition applicability for this Policy.</span></span>|
|<span data-ttu-id="f710a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f710a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f710a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f710a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f710a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f710a-158">The OS version applicability rule for this Policy.</span></span>|
|<span data-ttu-id="f710a-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="f710a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f710a-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="f710a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f710a-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f710a-161">The device mode applicability rule for this Policy.</span></span>|
|<span data-ttu-id="f710a-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f710a-162">createdDateTime</span></span>|<span data-ttu-id="f710a-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f710a-163">DateTimeOffset</span></span>|<span data-ttu-id="f710a-164">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f710a-164">DateTime the object was created.</span></span>|
|<span data-ttu-id="f710a-165">description</span><span class="sxs-lookup"><span data-stu-id="f710a-165">description</span></span>|<span data-ttu-id="f710a-166">String</span><span class="sxs-lookup"><span data-stu-id="f710a-166">String</span></span>|<span data-ttu-id="f710a-167">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-167">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f710a-168">displayName</span><span class="sxs-lookup"><span data-stu-id="f710a-168">displayName</span></span>|<span data-ttu-id="f710a-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f710a-169">String</span></span>|<span data-ttu-id="f710a-170">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-170">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f710a-171">version</span><span class="sxs-lookup"><span data-stu-id="f710a-171">version</span></span>|<span data-ttu-id="f710a-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f710a-172">Int32</span></span>|<span data-ttu-id="f710a-173">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-173">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f710a-174">Отношения</span><span class="sxs-lookup"><span data-stu-id="f710a-174">Relationships</span></span>
|<span data-ttu-id="f710a-175">Отношение</span><span class="sxs-lookup"><span data-stu-id="f710a-175">Relationship</span></span>|<span data-ttu-id="f710a-176">Тип</span><span class="sxs-lookup"><span data-stu-id="f710a-176">Type</span></span>|<span data-ttu-id="f710a-177">Описание</span><span class="sxs-lookup"><span data-stu-id="f710a-177">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f710a-178">**Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="f710a-178">**Device configuration**</span></span>|
|<span data-ttu-id="f710a-179">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="f710a-179">groupAssignments</span></span>|<span data-ttu-id="f710a-180">Коллекция deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f710a-180">deviceConfigurationGroupAssignment collection</span></span>|<span data-ttu-id="f710a-181">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-181">The list of group assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="f710a-182">assignments</span><span class="sxs-lookup"><span data-stu-id="f710a-182">assignments</span></span>|<span data-ttu-id="f710a-183">Коллекция объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f710a-183">deviceConfigurationAssignment collection</span></span>|<span data-ttu-id="f710a-184">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-184">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="f710a-185">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f710a-185">deviceStatuses</span></span>|<span data-ttu-id="f710a-186">Коллекция deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f710a-186">deviceConfigurationDeviceStatus collection</span></span>|<span data-ttu-id="f710a-187">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="f710a-187">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="f710a-188">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f710a-188">userStatuses</span></span>|<span data-ttu-id="f710a-189">Коллекция deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="f710a-189">deviceConfigurationUserStatus collection</span></span>|<span data-ttu-id="f710a-190">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="f710a-190">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="f710a-191">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f710a-191">deviceStatusOverview</span></span>|<span data-ttu-id="f710a-192">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f710a-192">deviceConfigurationDeviceOverview</span></span>|<span data-ttu-id="f710a-193">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="f710a-193">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="f710a-194">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f710a-194">userStatusOverview</span></span>|<span data-ttu-id="f710a-195">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f710a-195">deviceConfigurationUserOverview</span></span>|<span data-ttu-id="f710a-196">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="f710a-196">Device Configuration users status overview</span></span>|
|<span data-ttu-id="f710a-197">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f710a-197">deviceSettingStateSummaries</span></span>|<span data-ttu-id="f710a-198">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f710a-198">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f710a-199">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="f710a-199">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f710a-200">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f710a-200">JSON Representation</span></span>
<span data-ttu-id="f710a-201">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f710a-201">Here is a JSON representation of the resource.</span></span>
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



