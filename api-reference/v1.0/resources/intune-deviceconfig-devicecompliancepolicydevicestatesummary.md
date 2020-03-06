---
title: Тип ресурса deviceCompliancePolicyDeviceStateSummary
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 73609ae16400dbb36b14cedd6eb07646530c7a45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532603"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="967c5-103">Тип ресурса deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="967c5-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

<span data-ttu-id="967c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="967c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="967c5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="967c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="967c5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="967c5-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="967c5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="967c5-107">Methods</span></span>
|<span data-ttu-id="967c5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="967c5-108">Method</span></span>|<span data-ttu-id="967c5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="967c5-109">Return Type</span></span>|<span data-ttu-id="967c5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="967c5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="967c5-111">Получение объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="967c5-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|<span data-ttu-id="967c5-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md);</span><span class="sxs-lookup"><span data-stu-id="967c5-112">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)</span></span>|<span data-ttu-id="967c5-113">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="967c5-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="967c5-114">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="967c5-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="967c5-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="967c5-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="967c5-116">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="967c5-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="967c5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="967c5-117">Properties</span></span>
|<span data-ttu-id="967c5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="967c5-118">Property</span></span>|<span data-ttu-id="967c5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="967c5-119">Type</span></span>|<span data-ttu-id="967c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="967c5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="967c5-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="967c5-121">inGracePeriodCount</span></span>|<span data-ttu-id="967c5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-122">Int32</span></span>|<span data-ttu-id="967c5-123">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="967c5-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="967c5-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="967c5-124">configManagerCount</span></span>|<span data-ttu-id="967c5-125">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-125">Int32</span></span>|<span data-ttu-id="967c5-126">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="967c5-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="967c5-127">id</span><span class="sxs-lookup"><span data-stu-id="967c5-127">id</span></span>|<span data-ttu-id="967c5-128">Строка</span><span class="sxs-lookup"><span data-stu-id="967c5-128">String</span></span>|<span data-ttu-id="967c5-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="967c5-129">Key of the entity.</span></span>|
|<span data-ttu-id="967c5-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-130">unknownDeviceCount</span></span>|<span data-ttu-id="967c5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-131">Int32</span></span>|<span data-ttu-id="967c5-132">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="967c5-132">Number of unknown devices</span></span>|
|<span data-ttu-id="967c5-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="967c5-134">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-134">Int32</span></span>|<span data-ttu-id="967c5-135">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="967c5-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="967c5-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-136">compliantDeviceCount</span></span>|<span data-ttu-id="967c5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-137">Int32</span></span>|<span data-ttu-id="967c5-138">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="967c5-138">Number of compliant devices</span></span>|
|<span data-ttu-id="967c5-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-139">remediatedDeviceCount</span></span>|<span data-ttu-id="967c5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-140">Int32</span></span>|<span data-ttu-id="967c5-141">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="967c5-141">Number of remediated devices</span></span>|
|<span data-ttu-id="967c5-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="967c5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-143">Int32</span></span>|<span data-ttu-id="967c5-144">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="967c5-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="967c5-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-145">errorDeviceCount</span></span>|<span data-ttu-id="967c5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-146">Int32</span></span>|<span data-ttu-id="967c5-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="967c5-147">Number of error devices</span></span>|
|<span data-ttu-id="967c5-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="967c5-148">conflictDeviceCount</span></span>|<span data-ttu-id="967c5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="967c5-149">Int32</span></span>|<span data-ttu-id="967c5-150">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="967c5-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="967c5-151">Связи</span><span class="sxs-lookup"><span data-stu-id="967c5-151">Relationships</span></span>
<span data-ttu-id="967c5-152">Нет</span><span class="sxs-lookup"><span data-stu-id="967c5-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="967c5-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="967c5-153">JSON Representation</span></span>
<span data-ttu-id="967c5-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="967c5-154">Here is a JSON representation of the resource.</span></span>
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




