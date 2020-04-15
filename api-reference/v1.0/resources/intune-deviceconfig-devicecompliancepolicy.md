---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb96d3ff8dee50413b36cf70e8cfaf4b6f418cb0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448893"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="7de68-104">Тип ресурса deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7de68-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="7de68-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7de68-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7de68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7de68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7de68-107">Это базовый класс для политик обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="7de68-107">This is the base class for Compliance policy.</span></span> <span data-ttu-id="7de68-108">Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса.</span><span class="sxs-lookup"><span data-stu-id="7de68-108">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="7de68-109">Методы</span><span class="sxs-lookup"><span data-stu-id="7de68-109">Methods</span></span>
|<span data-ttu-id="7de68-110">Метод</span><span class="sxs-lookup"><span data-stu-id="7de68-110">Method</span></span>|<span data-ttu-id="7de68-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7de68-111">Return Type</span></span>|<span data-ttu-id="7de68-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7de68-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7de68-113">Перечисление deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="7de68-113">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="7de68-114">Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-114">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="7de68-115">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7de68-115">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="7de68-116">Получение deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7de68-116">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="7de68-117">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="7de68-117">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="7de68-118">Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7de68-118">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="7de68-119">Действие assign</span><span class="sxs-lookup"><span data-stu-id="7de68-119">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="7de68-120">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-120">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7de68-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7de68-121">Not yet documented</span></span>|
|[<span data-ttu-id="7de68-122">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="7de68-122">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="7de68-123">None</span><span class="sxs-lookup"><span data-stu-id="7de68-123">None</span></span>|<span data-ttu-id="7de68-124">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="7de68-124">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7de68-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="7de68-125">Properties</span></span>
|<span data-ttu-id="7de68-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7de68-126">Property</span></span>|<span data-ttu-id="7de68-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7de68-127">Type</span></span>|<span data-ttu-id="7de68-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7de68-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de68-129">id</span><span class="sxs-lookup"><span data-stu-id="7de68-129">id</span></span>|<span data-ttu-id="7de68-130">String</span><span class="sxs-lookup"><span data-stu-id="7de68-130">String</span></span>|<span data-ttu-id="7de68-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7de68-131">Key of the entity.</span></span>|
|<span data-ttu-id="7de68-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7de68-132">createdDateTime</span></span>|<span data-ttu-id="7de68-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7de68-133">DateTimeOffset</span></span>|<span data-ttu-id="7de68-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7de68-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="7de68-135">description</span><span class="sxs-lookup"><span data-stu-id="7de68-135">description</span></span>|<span data-ttu-id="7de68-136">String</span><span class="sxs-lookup"><span data-stu-id="7de68-136">String</span></span>|<span data-ttu-id="7de68-137">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7de68-137">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7de68-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7de68-138">lastModifiedDateTime</span></span>|<span data-ttu-id="7de68-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7de68-139">DateTimeOffset</span></span>|<span data-ttu-id="7de68-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7de68-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7de68-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7de68-141">displayName</span></span>|<span data-ttu-id="7de68-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7de68-142">String</span></span>|<span data-ttu-id="7de68-143">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7de68-143">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7de68-144">version</span><span class="sxs-lookup"><span data-stu-id="7de68-144">version</span></span>|<span data-ttu-id="7de68-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7de68-145">Int32</span></span>|<span data-ttu-id="7de68-146">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7de68-146">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7de68-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="7de68-147">Relationships</span></span>
|<span data-ttu-id="7de68-148">Связь</span><span class="sxs-lookup"><span data-stu-id="7de68-148">Relationship</span></span>|<span data-ttu-id="7de68-149">Тип</span><span class="sxs-lookup"><span data-stu-id="7de68-149">Type</span></span>|<span data-ttu-id="7de68-150">Описание</span><span class="sxs-lookup"><span data-stu-id="7de68-150">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de68-151">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="7de68-151">scheduledActionsForRule</span></span>|<span data-ttu-id="7de68-152">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-152">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="7de68-153">Список запланированных действий для этого правила.</span><span class="sxs-lookup"><span data-stu-id="7de68-153">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="7de68-154">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7de68-154">deviceStatuses</span></span>|<span data-ttu-id="7de68-155">Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-155">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="7de68-156">Список DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="7de68-156">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="7de68-157">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7de68-157">userStatuses</span></span>|<span data-ttu-id="7de68-158">Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-158">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="7de68-159">Список DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="7de68-159">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="7de68-160">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7de68-160">deviceStatusOverview</span></span>|[<span data-ttu-id="7de68-161">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7de68-161">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="7de68-162">Обзор состояния соответствия требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="7de68-162">Device compliance devices status overview</span></span>|
|<span data-ttu-id="7de68-163">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7de68-163">userStatusOverview</span></span>|[<span data-ttu-id="7de68-164">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="7de68-164">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="7de68-165">Обзор состояния соответствия требованиям устройств для пользователей.</span><span class="sxs-lookup"><span data-stu-id="7de68-165">Device compliance users status overview</span></span>|
|<span data-ttu-id="7de68-166">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7de68-166">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7de68-167">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-167">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7de68-168">Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.</span><span class="sxs-lookup"><span data-stu-id="7de68-168">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="7de68-169">assignments</span><span class="sxs-lookup"><span data-stu-id="7de68-169">assignments</span></span>|<span data-ttu-id="7de68-170">Коллекция объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7de68-170">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7de68-171">Коллекция назначений для этой политики обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="7de68-171">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7de68-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7de68-172">JSON Representation</span></span>
<span data-ttu-id="7de68-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7de68-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```







