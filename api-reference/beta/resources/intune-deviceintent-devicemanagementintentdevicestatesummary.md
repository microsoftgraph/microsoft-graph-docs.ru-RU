---
title: Тип ресурса Девицеманажементинтентдевицестатесуммари
description: Сущность, представляющая сводную информацию о состоянии устройства для намерения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9e0d8af7992248114364d7bdf4c2c34d2c715b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943385"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="10464-103">Тип ресурса Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="10464-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="10464-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10464-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10464-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10464-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10464-106">Сущность, представляющая сводную информацию о состоянии устройства для намерения</span><span class="sxs-lookup"><span data-stu-id="10464-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="10464-107">Методы</span><span class="sxs-lookup"><span data-stu-id="10464-107">Methods</span></span>
|<span data-ttu-id="10464-108">Метод</span><span class="sxs-lookup"><span data-stu-id="10464-108">Method</span></span>|<span data-ttu-id="10464-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="10464-109">Return Type</span></span>|<span data-ttu-id="10464-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10464-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10464-111">Получение Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="10464-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="10464-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="10464-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="10464-113">Чтение свойств и связей объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="10464-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="10464-114">Обновление Девицеманажементинтентдевицестатесуммари</span><span class="sxs-lookup"><span data-stu-id="10464-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="10464-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="10464-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="10464-116">Обновление свойств объекта [девицеманажементинтентдевицестатесуммари](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="10464-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10464-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="10464-117">Properties</span></span>
|<span data-ttu-id="10464-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="10464-118">Property</span></span>|<span data-ttu-id="10464-119">Тип</span><span class="sxs-lookup"><span data-stu-id="10464-119">Type</span></span>|<span data-ttu-id="10464-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10464-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10464-121">id</span><span class="sxs-lookup"><span data-stu-id="10464-121">id</span></span>|<span data-ttu-id="10464-122">Строка</span><span class="sxs-lookup"><span data-stu-id="10464-122">String</span></span>|<span data-ttu-id="10464-123">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="10464-123">The ID</span></span>|
|<span data-ttu-id="10464-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="10464-124">conflictCount</span></span>|<span data-ttu-id="10464-125">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-125">Int32</span></span>|<span data-ttu-id="10464-126">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="10464-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="10464-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="10464-127">errorCount</span></span>|<span data-ttu-id="10464-128">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-128">Int32</span></span>|<span data-ttu-id="10464-129">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="10464-129">Number of error devices</span></span>|
|<span data-ttu-id="10464-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="10464-130">failedCount</span></span>|<span data-ttu-id="10464-131">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-131">Int32</span></span>|<span data-ttu-id="10464-132">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="10464-132">Number of failed devices</span></span>|
|<span data-ttu-id="10464-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="10464-133">notApplicableCount</span></span>|<span data-ttu-id="10464-134">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-134">Int32</span></span>|<span data-ttu-id="10464-135">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="10464-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="10464-136">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="10464-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="10464-137">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-137">Int32</span></span>|<span data-ttu-id="10464-138">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="10464-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="10464-139">successCount</span><span class="sxs-lookup"><span data-stu-id="10464-139">successCount</span></span>|<span data-ttu-id="10464-140">Int32</span><span class="sxs-lookup"><span data-stu-id="10464-140">Int32</span></span>|<span data-ttu-id="10464-141">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="10464-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="10464-142">Связи</span><span class="sxs-lookup"><span data-stu-id="10464-142">Relationships</span></span>
<span data-ttu-id="10464-143">Нет</span><span class="sxs-lookup"><span data-stu-id="10464-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10464-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10464-144">JSON Representation</span></span>
<span data-ttu-id="10464-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10464-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```




