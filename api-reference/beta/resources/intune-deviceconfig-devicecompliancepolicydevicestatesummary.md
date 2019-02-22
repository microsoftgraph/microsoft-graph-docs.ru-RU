---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83e9279c819ad928afc1c0e7c7ddc9bd5ba87a5a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145796"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="23392-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="23392-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="23392-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23392-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23392-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23392-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="23392-107">Методы</span><span class="sxs-lookup"><span data-stu-id="23392-107">Methods</span></span>
|<span data-ttu-id="23392-108">Метод</span><span class="sxs-lookup"><span data-stu-id="23392-108">Method</span></span>|<span data-ttu-id="23392-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23392-109">Return Type</span></span>|<span data-ttu-id="23392-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23392-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23392-111">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="23392-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|<span data-ttu-id="23392-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md);</span><span class="sxs-lookup"><span data-stu-id="23392-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)</span></span>|<span data-ttu-id="23392-113">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="23392-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="23392-114">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="23392-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="23392-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="23392-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="23392-116">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="23392-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23392-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="23392-117">Properties</span></span>
|<span data-ttu-id="23392-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="23392-118">Property</span></span>|<span data-ttu-id="23392-119">Тип</span><span class="sxs-lookup"><span data-stu-id="23392-119">Type</span></span>|<span data-ttu-id="23392-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23392-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23392-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="23392-121">inGracePeriodCount</span></span>|<span data-ttu-id="23392-122">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-122">Int32</span></span>|<span data-ttu-id="23392-123">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="23392-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="23392-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="23392-124">configManagerCount</span></span>|<span data-ttu-id="23392-125">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-125">Int32</span></span>|<span data-ttu-id="23392-126">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="23392-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="23392-127">id</span><span class="sxs-lookup"><span data-stu-id="23392-127">id</span></span>|<span data-ttu-id="23392-128">String</span><span class="sxs-lookup"><span data-stu-id="23392-128">String</span></span>|<span data-ttu-id="23392-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="23392-129">Key of the entity.</span></span>|
|<span data-ttu-id="23392-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-130">unknownDeviceCount</span></span>|<span data-ttu-id="23392-131">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-131">Int32</span></span>|<span data-ttu-id="23392-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="23392-132">Number of unknown devices</span></span>|
|<span data-ttu-id="23392-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="23392-134">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-134">Int32</span></span>|<span data-ttu-id="23392-135">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="23392-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="23392-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-136">compliantDeviceCount</span></span>|<span data-ttu-id="23392-137">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-137">Int32</span></span>|<span data-ttu-id="23392-138">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="23392-138">Number of compliant devices</span></span>|
|<span data-ttu-id="23392-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-139">remediatedDeviceCount</span></span>|<span data-ttu-id="23392-140">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-140">Int32</span></span>|<span data-ttu-id="23392-141">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="23392-141">Number of remediated devices</span></span>|
|<span data-ttu-id="23392-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="23392-143">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-143">Int32</span></span>|<span data-ttu-id="23392-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="23392-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="23392-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-145">errorDeviceCount</span></span>|<span data-ttu-id="23392-146">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-146">Int32</span></span>|<span data-ttu-id="23392-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="23392-147">Number of error devices</span></span>|
|<span data-ttu-id="23392-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23392-148">conflictDeviceCount</span></span>|<span data-ttu-id="23392-149">Int32</span><span class="sxs-lookup"><span data-stu-id="23392-149">Int32</span></span>|<span data-ttu-id="23392-150">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="23392-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="23392-151">Связи</span><span class="sxs-lookup"><span data-stu-id="23392-151">Relationships</span></span>
<span data-ttu-id="23392-152">Нет</span><span class="sxs-lookup"><span data-stu-id="23392-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23392-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23392-153">JSON Representation</span></span>
<span data-ttu-id="23392-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23392-154">Here is a JSON representation of the resource.</span></span>
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




