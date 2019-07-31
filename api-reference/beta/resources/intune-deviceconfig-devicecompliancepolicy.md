---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffce3853157f5852c7ebf984ff0dfeea18fc2aef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970579"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="c40fb-104">Тип ресурса deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c40fb-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="c40fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c40fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c40fb-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c40fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c40fb-107">Это базовый класс для политик обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c40fb-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="c40fb-108">Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса.</span><span class="sxs-lookup"><span data-stu-id="c40fb-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="c40fb-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c40fb-109">Methods</span></span>
|<span data-ttu-id="c40fb-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c40fb-110">Method</span></span>|<span data-ttu-id="c40fb-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c40fb-111">Return Type</span></span>|<span data-ttu-id="c40fb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c40fb-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c40fb-113">Перечисление deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c40fb-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="c40fb-114">Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="c40fb-115">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c40fb-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="c40fb-116">Получение deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c40fb-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="c40fb-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c40fb-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="c40fb-118">Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c40fb-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="c40fb-119">Действие assign</span><span class="sxs-lookup"><span data-stu-id="c40fb-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="c40fb-120">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c40fb-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c40fb-121">Not yet documented</span></span>|
|[<span data-ttu-id="c40fb-122">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="c40fb-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="c40fb-123">None</span><span class="sxs-lookup"><span data-stu-id="c40fb-123">None</span></span>|<span data-ttu-id="c40fb-124">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="c40fb-124">Not yet documented</span></span>|
|[<span data-ttu-id="c40fb-125">Действие refreshDeviceComplianceReportSummarization</span><span class="sxs-lookup"><span data-stu-id="c40fb-125">refreshDeviceComplianceReportSummarization action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)|<span data-ttu-id="c40fb-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c40fb-126">None</span></span>|<span data-ttu-id="c40fb-127">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="c40fb-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c40fb-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="c40fb-128">Properties</span></span>
|<span data-ttu-id="c40fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c40fb-129">Property</span></span>|<span data-ttu-id="c40fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c40fb-130">Type</span></span>|<span data-ttu-id="c40fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c40fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40fb-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c40fb-132">roleScopeTagIds</span></span>|<span data-ttu-id="c40fb-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c40fb-133">String collection</span></span>|<span data-ttu-id="c40fb-134">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c40fb-134">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="c40fb-135">id</span><span class="sxs-lookup"><span data-stu-id="c40fb-135">id</span></span>|<span data-ttu-id="c40fb-136">String</span><span class="sxs-lookup"><span data-stu-id="c40fb-136">String</span></span>|<span data-ttu-id="c40fb-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c40fb-137">Key of the entity.</span></span>|
|<span data-ttu-id="c40fb-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c40fb-138">createdDateTime</span></span>|<span data-ttu-id="c40fb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40fb-139">DateTimeOffset</span></span>|<span data-ttu-id="c40fb-140">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c40fb-140">DateTime the object was created.</span></span>|
|<span data-ttu-id="c40fb-141">description</span><span class="sxs-lookup"><span data-stu-id="c40fb-141">description</span></span>|<span data-ttu-id="c40fb-142">String</span><span class="sxs-lookup"><span data-stu-id="c40fb-142">String</span></span>|<span data-ttu-id="c40fb-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c40fb-143">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c40fb-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c40fb-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c40fb-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40fb-145">DateTimeOffset</span></span>|<span data-ttu-id="c40fb-146">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c40fb-146">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c40fb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c40fb-147">displayName</span></span>|<span data-ttu-id="c40fb-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c40fb-148">String</span></span>|<span data-ttu-id="c40fb-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c40fb-149">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c40fb-150">version</span><span class="sxs-lookup"><span data-stu-id="c40fb-150">version</span></span>|<span data-ttu-id="c40fb-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c40fb-151">Int32</span></span>|<span data-ttu-id="c40fb-152">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c40fb-152">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c40fb-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="c40fb-153">Relationships</span></span>
|<span data-ttu-id="c40fb-154">Отношение</span><span class="sxs-lookup"><span data-stu-id="c40fb-154">Relationship</span></span>|<span data-ttu-id="c40fb-155">Тип</span><span class="sxs-lookup"><span data-stu-id="c40fb-155">Type</span></span>|<span data-ttu-id="c40fb-156">Описание</span><span class="sxs-lookup"><span data-stu-id="c40fb-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40fb-157">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="c40fb-157">scheduledActionsForRule</span></span>|<span data-ttu-id="c40fb-158">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-158">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="c40fb-159">Список запланированных действий для этого правила.</span><span class="sxs-lookup"><span data-stu-id="c40fb-159">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="c40fb-160">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c40fb-160">deviceStatuses</span></span>|<span data-ttu-id="c40fb-161">Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-161">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="c40fb-162">Список DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="c40fb-162">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="c40fb-163">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c40fb-163">userStatuses</span></span>|<span data-ttu-id="c40fb-164">Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-164">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="c40fb-165">Список DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c40fb-165">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="c40fb-166">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c40fb-166">deviceStatusOverview</span></span>|[<span data-ttu-id="c40fb-167">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c40fb-167">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c40fb-168">Обзор состояния соответствия требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="c40fb-168">Device compliance devices status overview</span></span>|
|<span data-ttu-id="c40fb-169">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c40fb-169">userStatusOverview</span></span>|[<span data-ttu-id="c40fb-170">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="c40fb-170">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="c40fb-171">Обзор состояния соответствия требованиям устройств для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c40fb-171">Device compliance users status overview</span></span>|
|<span data-ttu-id="c40fb-172">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c40fb-172">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c40fb-173">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-173">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c40fb-174">Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.</span><span class="sxs-lookup"><span data-stu-id="c40fb-174">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="c40fb-175">assignments</span><span class="sxs-lookup"><span data-stu-id="c40fb-175">assignments</span></span>|<span data-ttu-id="c40fb-176">Коллекция объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c40fb-176">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c40fb-177">Коллекция назначений для этой политики обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c40fb-177">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c40fb-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c40fb-178">JSON Representation</span></span>
<span data-ttu-id="c40fb-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c40fb-179">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





