---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0326b33fa4fa421d327542cabf80c45c4e8ef648
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448871"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="ed8ec-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed8ec-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="ed8ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed8ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed8ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed8ec-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ed8ec-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="ed8ec-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ed8ec-107">Methods</span></span>
|<span data-ttu-id="ed8ec-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ed8ec-108">Method</span></span>|<span data-ttu-id="ed8ec-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed8ec-109">Return Type</span></span>|<span data-ttu-id="ed8ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed8ec-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed8ec-111">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed8ec-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|<span data-ttu-id="ed8ec-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md);</span><span class="sxs-lookup"><span data-stu-id="ed8ec-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)</span></span>|<span data-ttu-id="ed8ec-113">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed8ec-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="ed8ec-114">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed8ec-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="ed8ec-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed8ec-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="ed8ec-116">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed8ec-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed8ec-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed8ec-117">Properties</span></span>
|<span data-ttu-id="ed8ec-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed8ec-118">Property</span></span>|<span data-ttu-id="ed8ec-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ed8ec-119">Type</span></span>|<span data-ttu-id="ed8ec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed8ec-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed8ec-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-121">inGracePeriodCount</span></span>|<span data-ttu-id="ed8ec-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-122">Int32</span></span>|<span data-ttu-id="ed8ec-123">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="ed8ec-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-124">configManagerCount</span></span>|<span data-ttu-id="ed8ec-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-125">Int32</span></span>|<span data-ttu-id="ed8ec-126">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="ed8ec-127">id</span><span class="sxs-lookup"><span data-stu-id="ed8ec-127">id</span></span>|<span data-ttu-id="ed8ec-128">String</span><span class="sxs-lookup"><span data-stu-id="ed8ec-128">String</span></span>|<span data-ttu-id="ed8ec-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-129">Key of the entity.</span></span>|
|<span data-ttu-id="ed8ec-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-130">unknownDeviceCount</span></span>|<span data-ttu-id="ed8ec-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-131">Int32</span></span>|<span data-ttu-id="ed8ec-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-132">Number of unknown devices</span></span>|
|<span data-ttu-id="ed8ec-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="ed8ec-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-134">Int32</span></span>|<span data-ttu-id="ed8ec-135">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="ed8ec-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-136">compliantDeviceCount</span></span>|<span data-ttu-id="ed8ec-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-137">Int32</span></span>|<span data-ttu-id="ed8ec-138">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-138">Number of compliant devices</span></span>|
|<span data-ttu-id="ed8ec-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-139">remediatedDeviceCount</span></span>|<span data-ttu-id="ed8ec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-140">Int32</span></span>|<span data-ttu-id="ed8ec-141">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-141">Number of remediated devices</span></span>|
|<span data-ttu-id="ed8ec-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ed8ec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-143">Int32</span></span>|<span data-ttu-id="ed8ec-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ed8ec-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-145">errorDeviceCount</span></span>|<span data-ttu-id="ed8ec-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-146">Int32</span></span>|<span data-ttu-id="ed8ec-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-147">Number of error devices</span></span>|
|<span data-ttu-id="ed8ec-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed8ec-148">conflictDeviceCount</span></span>|<span data-ttu-id="ed8ec-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ed8ec-149">Int32</span></span>|<span data-ttu-id="ed8ec-150">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="ed8ec-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed8ec-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="ed8ec-151">Relationships</span></span>
<span data-ttu-id="ed8ec-152">Нет</span><span class="sxs-lookup"><span data-stu-id="ed8ec-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed8ec-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed8ec-153">JSON Representation</span></span>
<span data-ttu-id="ed8ec-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed8ec-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```







