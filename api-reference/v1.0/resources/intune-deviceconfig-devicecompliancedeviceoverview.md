---
title: Тип ресурса deviceComplianceDeviceOverview
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 93da95ad7bb4360ab7e0a1b163c83f0b206a5644
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953030"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a><span data-ttu-id="8ba08-103">Тип ресурса deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ba08-103">deviceComplianceDeviceOverview resource type</span></span>

> <span data-ttu-id="8ba08-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ba08-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ba08-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8ba08-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="8ba08-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8ba08-106">Methods</span></span>
|<span data-ttu-id="8ba08-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8ba08-107">Method</span></span>|<span data-ttu-id="8ba08-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ba08-108">Return Type</span></span>|<span data-ttu-id="8ba08-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8ba08-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ba08-110">Получение объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ba08-110">Get deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[<span data-ttu-id="8ba08-111">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ba08-111">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="8ba08-112">Чтение свойств и связей объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8ba08-112">Read properties and relationships of the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="8ba08-113">Обновление объекта deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ba08-113">Update deviceComplianceDeviceOverview</span></span>](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[<span data-ttu-id="8ba08-114">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ba08-114">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="8ba08-115">Обновление свойств объекта [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8ba08-115">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ba08-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ba08-116">Properties</span></span>
|<span data-ttu-id="8ba08-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ba08-117">Property</span></span>|<span data-ttu-id="8ba08-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8ba08-118">Type</span></span>|<span data-ttu-id="8ba08-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8ba08-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba08-120">id</span><span class="sxs-lookup"><span data-stu-id="8ba08-120">id</span></span>|<span data-ttu-id="8ba08-121">String</span><span class="sxs-lookup"><span data-stu-id="8ba08-121">String</span></span>|<span data-ttu-id="8ba08-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ba08-122">Key of the entity.</span></span>|
|<span data-ttu-id="8ba08-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="8ba08-123">pendingCount</span></span>|<span data-ttu-id="8ba08-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-124">Int32</span></span>|<span data-ttu-id="8ba08-125">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="8ba08-125">Number of pending devices</span></span>|
|<span data-ttu-id="8ba08-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8ba08-126">notApplicableCount</span></span>|<span data-ttu-id="8ba08-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-127">Int32</span></span>|<span data-ttu-id="8ba08-128">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="8ba08-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="8ba08-129">successCount</span><span class="sxs-lookup"><span data-stu-id="8ba08-129">successCount</span></span>|<span data-ttu-id="8ba08-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-130">Int32</span></span>|<span data-ttu-id="8ba08-131">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="8ba08-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="8ba08-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="8ba08-132">errorCount</span></span>|<span data-ttu-id="8ba08-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-133">Int32</span></span>|<span data-ttu-id="8ba08-134">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="8ba08-134">Number of error devices</span></span>|
|<span data-ttu-id="8ba08-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="8ba08-135">failedCount</span></span>|<span data-ttu-id="8ba08-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-136">Int32</span></span>|<span data-ttu-id="8ba08-137">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="8ba08-137">Number of failed devices</span></span>|
|<span data-ttu-id="8ba08-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8ba08-138">lastUpdateDateTime</span></span>|<span data-ttu-id="8ba08-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ba08-139">DateTimeOffset</span></span>|<span data-ttu-id="8ba08-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="8ba08-140">Last update time</span></span>|
|<span data-ttu-id="8ba08-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="8ba08-141">configurationVersion</span></span>|<span data-ttu-id="8ba08-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba08-142">Int32</span></span>|<span data-ttu-id="8ba08-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="8ba08-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ba08-144">Связи</span><span class="sxs-lookup"><span data-stu-id="8ba08-144">Relationships</span></span>
<span data-ttu-id="8ba08-145">Нет</span><span class="sxs-lookup"><span data-stu-id="8ba08-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ba08-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ba08-146">JSON Representation</span></span>
<span data-ttu-id="8ba08-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ba08-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



