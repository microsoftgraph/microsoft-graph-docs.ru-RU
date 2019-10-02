---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b6d74a558a09f22f3d01dbfb771c00311c4a2fd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359637"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="d9a04-104">Тип ресурса deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a04-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="d9a04-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9a04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a04-106">Это базовый класс для политик обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d9a04-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="d9a04-107">Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса.</span><span class="sxs-lookup"><span data-stu-id="d9a04-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="d9a04-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d9a04-108">Methods</span></span>
|<span data-ttu-id="d9a04-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d9a04-109">Method</span></span>|<span data-ttu-id="d9a04-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9a04-110">Return Type</span></span>|<span data-ttu-id="d9a04-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9a04-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9a04-112">Перечисление deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="d9a04-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="d9a04-113">Коллекция [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="d9a04-114">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9a04-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="d9a04-115">Получение deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a04-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="d9a04-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a04-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="d9a04-117">Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d9a04-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="d9a04-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="d9a04-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="d9a04-119">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d9a04-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d9a04-120">Not yet documented</span></span>|
|[<span data-ttu-id="d9a04-121">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="d9a04-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="d9a04-122">None</span><span class="sxs-lookup"><span data-stu-id="d9a04-122">None</span></span>|<span data-ttu-id="d9a04-123">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="d9a04-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d9a04-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9a04-124">Properties</span></span>
|<span data-ttu-id="d9a04-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9a04-125">Property</span></span>|<span data-ttu-id="d9a04-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d9a04-126">Type</span></span>|<span data-ttu-id="d9a04-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d9a04-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a04-128">id</span><span class="sxs-lookup"><span data-stu-id="d9a04-128">id</span></span>|<span data-ttu-id="d9a04-129">String</span><span class="sxs-lookup"><span data-stu-id="d9a04-129">String</span></span>|<span data-ttu-id="d9a04-130">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d9a04-130">Key of the entity.</span></span>|
|<span data-ttu-id="d9a04-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a04-131">createdDateTime</span></span>|<span data-ttu-id="d9a04-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a04-132">DateTimeOffset</span></span>|<span data-ttu-id="d9a04-133">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d9a04-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="d9a04-134">description</span><span class="sxs-lookup"><span data-stu-id="d9a04-134">description</span></span>|<span data-ttu-id="d9a04-135">String</span><span class="sxs-lookup"><span data-stu-id="d9a04-135">String</span></span>|<span data-ttu-id="d9a04-136">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9a04-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d9a04-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a04-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d9a04-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a04-138">DateTimeOffset</span></span>|<span data-ttu-id="d9a04-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d9a04-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d9a04-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d9a04-140">displayName</span></span>|<span data-ttu-id="d9a04-141">Строка</span><span class="sxs-lookup"><span data-stu-id="d9a04-141">String</span></span>|<span data-ttu-id="d9a04-142">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9a04-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d9a04-143">version</span><span class="sxs-lookup"><span data-stu-id="d9a04-143">version</span></span>|<span data-ttu-id="d9a04-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a04-144">Int32</span></span>|<span data-ttu-id="d9a04-145">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9a04-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a04-146">Связи</span><span class="sxs-lookup"><span data-stu-id="d9a04-146">Relationships</span></span>
|<span data-ttu-id="d9a04-147">Связь</span><span class="sxs-lookup"><span data-stu-id="d9a04-147">Relationship</span></span>|<span data-ttu-id="d9a04-148">Тип</span><span class="sxs-lookup"><span data-stu-id="d9a04-148">Type</span></span>|<span data-ttu-id="d9a04-149">Описание</span><span class="sxs-lookup"><span data-stu-id="d9a04-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a04-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="d9a04-150">scheduledActionsForRule</span></span>|<span data-ttu-id="d9a04-151">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="d9a04-152">Список запланированных действий для этого правила.</span><span class="sxs-lookup"><span data-stu-id="d9a04-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="d9a04-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d9a04-153">deviceStatuses</span></span>|<span data-ttu-id="d9a04-154">Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="d9a04-155">Список DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="d9a04-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="d9a04-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d9a04-156">userStatuses</span></span>|<span data-ttu-id="d9a04-157">Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="d9a04-158">Список DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="d9a04-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="d9a04-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d9a04-159">deviceStatusOverview</span></span>|[<span data-ttu-id="d9a04-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d9a04-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="d9a04-161">Обзор состояния соответствия требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="d9a04-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="d9a04-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d9a04-162">userStatusOverview</span></span>|[<span data-ttu-id="d9a04-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="d9a04-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="d9a04-164">Обзор состояния соответствия требованиям устройств для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d9a04-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="d9a04-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d9a04-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d9a04-166">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d9a04-167">Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.</span><span class="sxs-lookup"><span data-stu-id="d9a04-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="d9a04-168">assignments</span><span class="sxs-lookup"><span data-stu-id="d9a04-168">assignments</span></span>|<span data-ttu-id="d9a04-169">Коллекция объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9a04-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d9a04-170">Коллекция назначений для этой политики обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d9a04-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9a04-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9a04-171">JSON Representation</span></span>
<span data-ttu-id="d9a04-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9a04-172">Here is a JSON representation of the resource.</span></span>
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




