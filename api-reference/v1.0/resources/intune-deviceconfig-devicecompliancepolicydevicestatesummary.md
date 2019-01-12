---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c3f047f35718c2172ad5d04a17c07ba746012a2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912955"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="bb9d6-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb9d6-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="bb9d6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb9d6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bb9d6-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="bb9d6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bb9d6-106">Methods</span></span>
|<span data-ttu-id="bb9d6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bb9d6-107">Method</span></span>|<span data-ttu-id="bb9d6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb9d6-108">Return Type</span></span>|<span data-ttu-id="bb9d6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9d6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb9d6-110">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb9d6-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="bb9d6-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb9d6-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="bb9d6-112">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb9d6-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="bb9d6-113">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb9d6-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="bb9d6-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb9d6-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="bb9d6-115">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb9d6-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb9d6-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb9d6-116">Properties</span></span>
|<span data-ttu-id="bb9d6-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb9d6-117">Property</span></span>|<span data-ttu-id="bb9d6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9d6-118">Type</span></span>|<span data-ttu-id="bb9d6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9d6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb9d6-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-120">inGracePeriodCount</span></span>|<span data-ttu-id="bb9d6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-121">Int32</span></span>|<span data-ttu-id="bb9d6-122">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="bb9d6-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-123">configManagerCount</span></span>|<span data-ttu-id="bb9d6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-124">Int32</span></span>|<span data-ttu-id="bb9d6-125">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="bb9d6-126">id</span><span class="sxs-lookup"><span data-stu-id="bb9d6-126">id</span></span>|<span data-ttu-id="bb9d6-127">Строка</span><span class="sxs-lookup"><span data-stu-id="bb9d6-127">String</span></span>|<span data-ttu-id="bb9d6-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-128">Key of the entity.</span></span>|
|<span data-ttu-id="bb9d6-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-129">unknownDeviceCount</span></span>|<span data-ttu-id="bb9d6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-130">Int32</span></span>|<span data-ttu-id="bb9d6-131">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-131">Number of unknown devices</span></span>|
|<span data-ttu-id="bb9d6-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="bb9d6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-133">Int32</span></span>|<span data-ttu-id="bb9d6-134">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="bb9d6-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-135">compliantDeviceCount</span></span>|<span data-ttu-id="bb9d6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-136">Int32</span></span>|<span data-ttu-id="bb9d6-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-137">Number of compliant devices</span></span>|
|<span data-ttu-id="bb9d6-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-138">remediatedDeviceCount</span></span>|<span data-ttu-id="bb9d6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-139">Int32</span></span>|<span data-ttu-id="bb9d6-140">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-140">Number of remediated devices</span></span>|
|<span data-ttu-id="bb9d6-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bb9d6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-142">Int32</span></span>|<span data-ttu-id="bb9d6-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bb9d6-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-144">errorDeviceCount</span></span>|<span data-ttu-id="bb9d6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-145">Int32</span></span>|<span data-ttu-id="bb9d6-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-146">Number of error devices</span></span>|
|<span data-ttu-id="bb9d6-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb9d6-147">conflictDeviceCount</span></span>|<span data-ttu-id="bb9d6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bb9d6-148">Int32</span></span>|<span data-ttu-id="bb9d6-149">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="bb9d6-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb9d6-150">Связи</span><span class="sxs-lookup"><span data-stu-id="bb9d6-150">Relationships</span></span>
<span data-ttu-id="bb9d6-151">Нет</span><span class="sxs-lookup"><span data-stu-id="bb9d6-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bb9d6-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb9d6-152">JSON Representation</span></span>
<span data-ttu-id="bb9d6-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-153">Here is a JSON representation of the resource.</span></span>
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



