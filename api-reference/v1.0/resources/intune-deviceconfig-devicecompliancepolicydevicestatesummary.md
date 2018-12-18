---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 229a03830fec065cbed9861ad1db07418c3fbfa8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329017"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="f698f-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f698f-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="f698f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f698f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f698f-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f698f-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="f698f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f698f-106">Methods</span></span>
|<span data-ttu-id="f698f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f698f-107">Method</span></span>|<span data-ttu-id="f698f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f698f-108">Return Type</span></span>|<span data-ttu-id="f698f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f698f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f698f-110">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f698f-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="f698f-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f698f-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f698f-112">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f698f-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="f698f-113">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f698f-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="f698f-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f698f-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="f698f-115">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f698f-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f698f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="f698f-116">Properties</span></span>
|<span data-ttu-id="f698f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="f698f-117">Property</span></span>|<span data-ttu-id="f698f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f698f-118">Type</span></span>|<span data-ttu-id="f698f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f698f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f698f-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="f698f-120">inGracePeriodCount</span></span>|<span data-ttu-id="f698f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-121">Int32</span></span>|<span data-ttu-id="f698f-122">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="f698f-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="f698f-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="f698f-123">configManagerCount</span></span>|<span data-ttu-id="f698f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-124">Int32</span></span>|<span data-ttu-id="f698f-125">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="f698f-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="f698f-126">id</span><span class="sxs-lookup"><span data-stu-id="f698f-126">id</span></span>|<span data-ttu-id="f698f-127">Строка</span><span class="sxs-lookup"><span data-stu-id="f698f-127">String</span></span>|<span data-ttu-id="f698f-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f698f-128">Key of the entity.</span></span>|
|<span data-ttu-id="f698f-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-129">unknownDeviceCount</span></span>|<span data-ttu-id="f698f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-130">Int32</span></span>|<span data-ttu-id="f698f-131">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="f698f-131">Number of unknown devices</span></span>|
|<span data-ttu-id="f698f-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="f698f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-133">Int32</span></span>|<span data-ttu-id="f698f-134">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f698f-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="f698f-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-135">compliantDeviceCount</span></span>|<span data-ttu-id="f698f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-136">Int32</span></span>|<span data-ttu-id="f698f-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f698f-137">Number of compliant devices</span></span>|
|<span data-ttu-id="f698f-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-138">remediatedDeviceCount</span></span>|<span data-ttu-id="f698f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-139">Int32</span></span>|<span data-ttu-id="f698f-140">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f698f-140">Number of remediated devices</span></span>|
|<span data-ttu-id="f698f-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f698f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-142">Int32</span></span>|<span data-ttu-id="f698f-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="f698f-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f698f-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-144">errorDeviceCount</span></span>|<span data-ttu-id="f698f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-145">Int32</span></span>|<span data-ttu-id="f698f-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f698f-146">Number of error devices</span></span>|
|<span data-ttu-id="f698f-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f698f-147">conflictDeviceCount</span></span>|<span data-ttu-id="f698f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f698f-148">Int32</span></span>|<span data-ttu-id="f698f-149">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="f698f-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="f698f-150">Связи</span><span class="sxs-lookup"><span data-stu-id="f698f-150">Relationships</span></span>
<span data-ttu-id="f698f-151">Нет</span><span class="sxs-lookup"><span data-stu-id="f698f-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f698f-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f698f-152">JSON Representation</span></span>
<span data-ttu-id="f698f-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f698f-153">Here is a JSON representation of the resource.</span></span>
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



