---
title: Тип ресурса deviceCompliancePolicy
description: 'Это базовый класс для политик обеспечения соответствия требованиям. Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса. '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d642ee7466df61376917ddca413deb47d7a8b8d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060064"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="c7f7a-104">Тип ресурса deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7f7a-104">deviceCompliancePolicy resource type</span></span>

<span data-ttu-id="c7f7a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7f7a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7f7a-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7f7a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7f7a-108">Это базовый класс для политик обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-108">This is the base class for Compliance policy.</span></span> <span data-ttu-id="c7f7a-109">Такие политики предназначаются для определенной платформы. Отдельные политики обеспечения соответствия требованиям наследуются от этого класса.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-109">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="c7f7a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c7f7a-110">Methods</span></span>
|<span data-ttu-id="c7f7a-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c7f7a-111">Method</span></span>|<span data-ttu-id="c7f7a-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7f7a-112">Return Type</span></span>|<span data-ttu-id="c7f7a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f7a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7f7a-114">Перечисление deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="c7f7a-114">List deviceCompliancePolicies</span></span>](../api/intune-shared-devicecompliancepolicy-list.md)|<span data-ttu-id="c7f7a-115">Коллекция [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-115">[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="c7f7a-116">Список свойств и связей объектов [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7f7a-116">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="c7f7a-117">Получение deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7f7a-117">Get deviceCompliancePolicy</span></span>](../api/intune-shared-devicecompliancepolicy-get.md)|[<span data-ttu-id="c7f7a-118">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7f7a-118">deviceCompliancePolicy</span></span>](../resources/intune-shared-devicecompliancepolicy.md)|<span data-ttu-id="c7f7a-119">Считывание свойств и связей объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c7f7a-119">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) object.</span></span>|
|<span data-ttu-id="c7f7a-120">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="c7f7a-120">**Device configuration**</span></span>|
|[<span data-ttu-id="c7f7a-121">Действие assign</span><span class="sxs-lookup"><span data-stu-id="c7f7a-121">assign action</span></span>](../api/intune-shared-devicecompliancepolicy-assign.md)|<span data-ttu-id="c7f7a-122">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-122">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c7f7a-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c7f7a-123">Not yet documented</span></span>|
|<span data-ttu-id="c7f7a-124">Действие scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="c7f7a-124">scheduleActionsForRules action</span></span>|<span data-ttu-id="c7f7a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c7f7a-125">None</span></span>|<span data-ttu-id="c7f7a-126">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c7f7a-126">Not yet documented</span></span>|
|<span data-ttu-id="c7f7a-127">действие Рефрешдевицекомплианцерепортсуммаризатион] (.. /АПИ/интуне-Шаред-девицекомплианцеполици-рефрешдевицекомплианцерепортсуммаризатион.МД)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-127">refreshDeviceComplianceReportSummarization action](../api/intune-shared-devicecompliancepolicy-refreshdevicecompliancereportsummarization.md)</span></span>|<span data-ttu-id="c7f7a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c7f7a-128">None</span></span>|<span data-ttu-id="c7f7a-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c7f7a-129">Not yet documented</span></span>|
|<span data-ttu-id="c7f7a-130">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c7f7a-130">**Policy Set**</span></span>|
|[<span data-ttu-id="c7f7a-131">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="c7f7a-131">hasPayloadLinks action</span></span>](../api/intune-shared-devicecompliancepolicy-haspayloadlinks.md)|<span data-ttu-id="c7f7a-132">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-132">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="c7f7a-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c7f7a-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c7f7a-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7f7a-134">Properties</span></span>
|<span data-ttu-id="c7f7a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7f7a-135">Property</span></span>|<span data-ttu-id="c7f7a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="c7f7a-136">Type</span></span>|<span data-ttu-id="c7f7a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f7a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f7a-138">id</span><span class="sxs-lookup"><span data-stu-id="c7f7a-138">id</span></span>|<span data-ttu-id="c7f7a-139">String</span><span class="sxs-lookup"><span data-stu-id="c7f7a-139">String</span></span>|<span data-ttu-id="c7f7a-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-140">Key of the entity.</span></span>|
|<span data-ttu-id="c7f7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7f7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="c7f7a-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="c7f7a-142">String collection</span></span>|<span data-ttu-id="c7f7a-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-143">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="c7f7a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f7a-144">createdDateTime</span></span>|<span data-ttu-id="c7f7a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f7a-145">DateTimeOffset</span></span>|<span data-ttu-id="c7f7a-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-146">DateTime the object was created.</span></span>|
|<span data-ttu-id="c7f7a-147">description</span><span class="sxs-lookup"><span data-stu-id="c7f7a-147">description</span></span>|<span data-ttu-id="c7f7a-148">String</span><span class="sxs-lookup"><span data-stu-id="c7f7a-148">String</span></span>|<span data-ttu-id="c7f7a-149">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-149">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c7f7a-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7f7a-150">lastModifiedDateTime</span></span>|<span data-ttu-id="c7f7a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7f7a-151">DateTimeOffset</span></span>|<span data-ttu-id="c7f7a-152">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-152">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c7f7a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c7f7a-153">displayName</span></span>|<span data-ttu-id="c7f7a-154">String</span><span class="sxs-lookup"><span data-stu-id="c7f7a-154">String</span></span>|<span data-ttu-id="c7f7a-155">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-155">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c7f7a-156">version</span><span class="sxs-lookup"><span data-stu-id="c7f7a-156">version</span></span>|<span data-ttu-id="c7f7a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c7f7a-157">Int32</span></span>|<span data-ttu-id="c7f7a-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-158">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7f7a-159">Связи</span><span class="sxs-lookup"><span data-stu-id="c7f7a-159">Relationships</span></span>
|<span data-ttu-id="c7f7a-160">Связь</span><span class="sxs-lookup"><span data-stu-id="c7f7a-160">Relationship</span></span>|<span data-ttu-id="c7f7a-161">Тип</span><span class="sxs-lookup"><span data-stu-id="c7f7a-161">Type</span></span>|<span data-ttu-id="c7f7a-162">Описание</span><span class="sxs-lookup"><span data-stu-id="c7f7a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7f7a-163">**Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="c7f7a-163">**Device configuration**</span></span>|
|<span data-ttu-id="c7f7a-164">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="c7f7a-164">scheduledActionsForRule</span></span>|<span data-ttu-id="c7f7a-165">Коллекция [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-165">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="c7f7a-166">Список запланированных действий для этого правила.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-166">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="c7f7a-167">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c7f7a-167">deviceStatuses</span></span>|<span data-ttu-id="c7f7a-168">Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-168">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="c7f7a-169">Список DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-169">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="c7f7a-170">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c7f7a-170">userStatuses</span></span>|<span data-ttu-id="c7f7a-171">Коллекция [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-171">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="c7f7a-172">Список DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-172">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="c7f7a-173">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7f7a-173">deviceStatusOverview</span></span>|[<span data-ttu-id="c7f7a-174">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c7f7a-174">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="c7f7a-175">Обзор состояния соответствия требованиям устройств.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-175">Device compliance devices status overview</span></span>|
|<span data-ttu-id="c7f7a-176">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c7f7a-176">userStatusOverview</span></span>|[<span data-ttu-id="c7f7a-177">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="c7f7a-177">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="c7f7a-178">Обзор состояния соответствия требованиям устройств для пользователей.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-178">Device compliance users status overview</span></span>|
|<span data-ttu-id="c7f7a-179">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c7f7a-179">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c7f7a-180">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-180">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c7f7a-181">Сводка по состоянию параметров обеспечения соответствия требованиям для устройств.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-181">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="c7f7a-182">assignments</span><span class="sxs-lookup"><span data-stu-id="c7f7a-182">assignments</span></span>|<span data-ttu-id="c7f7a-183">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7f7a-183">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="c7f7a-184">Коллекция назначений для этой политики обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-184">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7f7a-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7f7a-185">JSON Representation</span></span>
<span data-ttu-id="c7f7a-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7f7a-186">Here is a JSON representation of the resource.</span></span>
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






