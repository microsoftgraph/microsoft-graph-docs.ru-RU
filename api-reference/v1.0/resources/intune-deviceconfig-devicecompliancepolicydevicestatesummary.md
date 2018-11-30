---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Н/Д
ms.openlocfilehash: 78bf38263dd203f8e9a4db359f29d0481b7a26c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024413"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="3b5b7-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b7-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="3b5b7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b5b7-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b5b7-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="3b5b7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3b5b7-106">Methods</span></span>
|<span data-ttu-id="3b5b7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3b5b7-107">Method</span></span>|<span data-ttu-id="3b5b7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b5b7-108">Return Type</span></span>|<span data-ttu-id="3b5b7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3b5b7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b5b7-110">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b7-110">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="3b5b7-111">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b7-111">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="3b5b7-112">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3b5b7-112">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="3b5b7-113">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b7-113">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="3b5b7-114">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b7-114">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="3b5b7-115">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3b5b7-115">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b5b7-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b5b7-116">Properties</span></span>
|<span data-ttu-id="3b5b7-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b5b7-117">Property</span></span>|<span data-ttu-id="3b5b7-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3b5b7-118">Type</span></span>|<span data-ttu-id="3b5b7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3b5b7-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b5b7-120">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-120">inGracePeriodCount</span></span>|<span data-ttu-id="3b5b7-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-121">Int32</span></span>|<span data-ttu-id="3b5b7-122">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-122">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="3b5b7-123">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-123">configManagerCount</span></span>|<span data-ttu-id="3b5b7-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-124">Int32</span></span>|<span data-ttu-id="3b5b7-125">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-125">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="3b5b7-126">id</span><span class="sxs-lookup"><span data-stu-id="3b5b7-126">id</span></span>|<span data-ttu-id="3b5b7-127">String</span><span class="sxs-lookup"><span data-stu-id="3b5b7-127">String</span></span>|<span data-ttu-id="3b5b7-128">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-128">Key of the entity.</span></span>|
|<span data-ttu-id="3b5b7-129">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-129">unknownDeviceCount</span></span>|<span data-ttu-id="3b5b7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-130">Int32</span></span>|<span data-ttu-id="3b5b7-131">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-131">Number of unknown devices</span></span>|
|<span data-ttu-id="3b5b7-132">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-132">notApplicableDeviceCount</span></span>|<span data-ttu-id="3b5b7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-133">Int32</span></span>|<span data-ttu-id="3b5b7-134">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-134">Number of not applicable devices</span></span>|
|<span data-ttu-id="3b5b7-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-135">compliantDeviceCount</span></span>|<span data-ttu-id="3b5b7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-136">Int32</span></span>|<span data-ttu-id="3b5b7-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-137">Number of compliant devices</span></span>|
|<span data-ttu-id="3b5b7-138">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-138">remediatedDeviceCount</span></span>|<span data-ttu-id="3b5b7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-139">Int32</span></span>|<span data-ttu-id="3b5b7-140">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-140">Number of remediated devices</span></span>|
|<span data-ttu-id="3b5b7-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3b5b7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-142">Int32</span></span>|<span data-ttu-id="3b5b7-143">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-143">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3b5b7-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-144">errorDeviceCount</span></span>|<span data-ttu-id="3b5b7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-145">Int32</span></span>|<span data-ttu-id="3b5b7-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-146">Number of error devices</span></span>|
|<span data-ttu-id="3b5b7-147">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3b5b7-147">conflictDeviceCount</span></span>|<span data-ttu-id="3b5b7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3b5b7-148">Int32</span></span>|<span data-ttu-id="3b5b7-149">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="3b5b7-149">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b5b7-150">Связи</span><span class="sxs-lookup"><span data-stu-id="3b5b7-150">Relationships</span></span>
<span data-ttu-id="3b5b7-151">Нет</span><span class="sxs-lookup"><span data-stu-id="3b5b7-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b5b7-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b5b7-152">JSON Representation</span></span>
<span data-ttu-id="3b5b7-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b5b7-153">Here is a JSON representation of the resource.</span></span>
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



