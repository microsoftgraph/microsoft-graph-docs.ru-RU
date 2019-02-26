---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c434009d1f34014a36e6871963051773aa2aab5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256877"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="78c86-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="78c86-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="78c86-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78c86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78c86-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="78c86-105">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="78c86-106">Методы</span><span class="sxs-lookup"><span data-stu-id="78c86-106">Methods</span></span>
|<span data-ttu-id="78c86-107">Метод</span><span class="sxs-lookup"><span data-stu-id="78c86-107">Method</span></span>|<span data-ttu-id="78c86-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78c86-108">Return Type</span></span>|<span data-ttu-id="78c86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78c86-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78c86-110">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="78c86-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|<span data-ttu-id="78c86-111">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md);</span><span class="sxs-lookup"><span data-stu-id="78c86-111">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)</span></span>|<span data-ttu-id="78c86-112">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="78c86-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="78c86-113">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="78c86-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="78c86-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="78c86-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="78c86-115">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="78c86-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78c86-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="78c86-116">Properties</span></span>
|<span data-ttu-id="78c86-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="78c86-117">Property</span></span>|<span data-ttu-id="78c86-118">Тип</span><span class="sxs-lookup"><span data-stu-id="78c86-118">Type</span></span>|<span data-ttu-id="78c86-119">Описание</span><span class="sxs-lookup"><span data-stu-id="78c86-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c86-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="78c86-120">inGracePeriodCount</span></span>|<span data-ttu-id="78c86-121">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-121">Int32</span></span>|<span data-ttu-id="78c86-122">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="78c86-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="78c86-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="78c86-123">configManagerCount</span></span>|<span data-ttu-id="78c86-124">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-124">Int32</span></span>|<span data-ttu-id="78c86-125">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="78c86-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="78c86-126">id</span><span class="sxs-lookup"><span data-stu-id="78c86-126">id</span></span>|<span data-ttu-id="78c86-127">String</span><span class="sxs-lookup"><span data-stu-id="78c86-127">String</span></span>|<span data-ttu-id="78c86-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="78c86-128">Key of the entity.</span></span>|
|<span data-ttu-id="78c86-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-129">unknownDeviceCount</span></span>|<span data-ttu-id="78c86-130">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-130">Int32</span></span>|<span data-ttu-id="78c86-131">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="78c86-131">Number of unknown devices</span></span>|
|<span data-ttu-id="78c86-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="78c86-133">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-133">Int32</span></span>|<span data-ttu-id="78c86-134">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="78c86-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="78c86-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-135">compliantDeviceCount</span></span>|<span data-ttu-id="78c86-136">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-136">Int32</span></span>|<span data-ttu-id="78c86-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="78c86-137">Number of compliant devices</span></span>|
|<span data-ttu-id="78c86-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-138">remediatedDeviceCount</span></span>|<span data-ttu-id="78c86-139">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-139">Int32</span></span>|<span data-ttu-id="78c86-140">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="78c86-140">Number of remediated devices</span></span>|
|<span data-ttu-id="78c86-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="78c86-142">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-142">Int32</span></span>|<span data-ttu-id="78c86-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="78c86-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="78c86-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-144">errorDeviceCount</span></span>|<span data-ttu-id="78c86-145">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-145">Int32</span></span>|<span data-ttu-id="78c86-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="78c86-146">Number of error devices</span></span>|
|<span data-ttu-id="78c86-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="78c86-147">conflictDeviceCount</span></span>|<span data-ttu-id="78c86-148">Int32</span><span class="sxs-lookup"><span data-stu-id="78c86-148">Int32</span></span>|<span data-ttu-id="78c86-149">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="78c86-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="78c86-150">Связи</span><span class="sxs-lookup"><span data-stu-id="78c86-150">Relationships</span></span>
<span data-ttu-id="78c86-151">Нет</span><span class="sxs-lookup"><span data-stu-id="78c86-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78c86-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78c86-152">JSON Representation</span></span>
<span data-ttu-id="78c86-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78c86-153">Here is a JSON representation of the resource.</span></span>
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



