---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b21b34506c9ef763751a32a4e83b9c7f5e363a19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815822"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="7552b-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7552b-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="7552b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7552b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7552b-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7552b-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="7552b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7552b-106">Methods</span></span>
|<span data-ttu-id="7552b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7552b-107">Method</span></span>|<span data-ttu-id="7552b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7552b-108">Return Type</span></span>|<span data-ttu-id="7552b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7552b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7552b-110">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7552b-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="7552b-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7552b-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="7552b-112">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7552b-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="7552b-113">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7552b-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="7552b-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7552b-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="7552b-115">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7552b-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7552b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7552b-116">Properties</span></span>
|<span data-ttu-id="7552b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="7552b-117">Property</span></span>|<span data-ttu-id="7552b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7552b-118">Type</span></span>|<span data-ttu-id="7552b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7552b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7552b-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="7552b-120">inGracePeriodCount</span></span>|<span data-ttu-id="7552b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-121">Int32</span></span>|<span data-ttu-id="7552b-122">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="7552b-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="7552b-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="7552b-123">configManagerCount</span></span>|<span data-ttu-id="7552b-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-124">Int32</span></span>|<span data-ttu-id="7552b-125">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="7552b-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="7552b-126">id</span><span class="sxs-lookup"><span data-stu-id="7552b-126">id</span></span>|<span data-ttu-id="7552b-127">Строка</span><span class="sxs-lookup"><span data-stu-id="7552b-127">String</span></span>|<span data-ttu-id="7552b-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7552b-128">Key of the entity.</span></span>|
|<span data-ttu-id="7552b-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-129">unknownDeviceCount</span></span>|<span data-ttu-id="7552b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-130">Int32</span></span>|<span data-ttu-id="7552b-131">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="7552b-131">Number of unknown devices</span></span>|
|<span data-ttu-id="7552b-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="7552b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-133">Int32</span></span>|<span data-ttu-id="7552b-134">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7552b-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="7552b-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-135">compliantDeviceCount</span></span>|<span data-ttu-id="7552b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-136">Int32</span></span>|<span data-ttu-id="7552b-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7552b-137">Number of compliant devices</span></span>|
|<span data-ttu-id="7552b-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-138">remediatedDeviceCount</span></span>|<span data-ttu-id="7552b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-139">Int32</span></span>|<span data-ttu-id="7552b-140">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7552b-140">Number of remediated devices</span></span>|
|<span data-ttu-id="7552b-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7552b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-142">Int32</span></span>|<span data-ttu-id="7552b-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7552b-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="7552b-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-144">errorDeviceCount</span></span>|<span data-ttu-id="7552b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-145">Int32</span></span>|<span data-ttu-id="7552b-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7552b-146">Number of error devices</span></span>|
|<span data-ttu-id="7552b-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7552b-147">conflictDeviceCount</span></span>|<span data-ttu-id="7552b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7552b-148">Int32</span></span>|<span data-ttu-id="7552b-149">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="7552b-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="7552b-150">Связи</span><span class="sxs-lookup"><span data-stu-id="7552b-150">Relationships</span></span>
<span data-ttu-id="7552b-151">Нет</span><span class="sxs-lookup"><span data-stu-id="7552b-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7552b-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7552b-152">JSON Representation</span></span>
<span data-ttu-id="7552b-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7552b-153">Here is a JSON representation of the resource.</span></span>
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



