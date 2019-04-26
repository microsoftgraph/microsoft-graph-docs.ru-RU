---
title: Тип ресурса deviceConfigurationDeviceOverview
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e6ded68974f3a4baa307d186e93ea83931f07aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567454"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="848ec-103">Тип ресурса deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="848ec-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="848ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="848ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="848ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="848ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="848ec-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="848ec-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="848ec-107">Методы</span><span class="sxs-lookup"><span data-stu-id="848ec-107">Methods</span></span>
|<span data-ttu-id="848ec-108">Метод</span><span class="sxs-lookup"><span data-stu-id="848ec-108">Method</span></span>|<span data-ttu-id="848ec-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="848ec-109">Return Type</span></span>|<span data-ttu-id="848ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="848ec-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="848ec-111">Получение объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="848ec-111">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="848ec-112">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="848ec-112">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="848ec-113">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="848ec-113">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="848ec-114">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="848ec-114">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="848ec-115">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="848ec-115">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="848ec-116">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="848ec-116">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="848ec-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="848ec-117">Properties</span></span>
|<span data-ttu-id="848ec-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="848ec-118">Property</span></span>|<span data-ttu-id="848ec-119">Тип</span><span class="sxs-lookup"><span data-stu-id="848ec-119">Type</span></span>|<span data-ttu-id="848ec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="848ec-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="848ec-121">id</span><span class="sxs-lookup"><span data-stu-id="848ec-121">id</span></span>|<span data-ttu-id="848ec-122">String</span><span class="sxs-lookup"><span data-stu-id="848ec-122">String</span></span>|<span data-ttu-id="848ec-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="848ec-123">Key of the entity.</span></span>|
|<span data-ttu-id="848ec-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="848ec-124">pendingCount</span></span>|<span data-ttu-id="848ec-125">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-125">Int32</span></span>|<span data-ttu-id="848ec-126">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="848ec-126">Number of pending devices</span></span>|
|<span data-ttu-id="848ec-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="848ec-127">notApplicableCount</span></span>|<span data-ttu-id="848ec-128">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-128">Int32</span></span>|<span data-ttu-id="848ec-129">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="848ec-129">Number of not applicable devices</span></span>|
|<span data-ttu-id="848ec-130">Свойства notapplicableplatformcount</span><span class="sxs-lookup"><span data-stu-id="848ec-130">notApplicablePlatformCount</span></span>|<span data-ttu-id="848ec-131">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-131">Int32</span></span>|<span data-ttu-id="848ec-132">Количество неприменимых устройств из-за несовпадения платформы и политики</span><span class="sxs-lookup"><span data-stu-id="848ec-132">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="848ec-133">successCount</span><span class="sxs-lookup"><span data-stu-id="848ec-133">successCount</span></span>|<span data-ttu-id="848ec-134">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-134">Int32</span></span>|<span data-ttu-id="848ec-135">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="848ec-135">Number of succeeded devices</span></span>|
|<span data-ttu-id="848ec-136">errorCount</span><span class="sxs-lookup"><span data-stu-id="848ec-136">errorCount</span></span>|<span data-ttu-id="848ec-137">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-137">Int32</span></span>|<span data-ttu-id="848ec-138">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="848ec-138">Number of error devices</span></span>|
|<span data-ttu-id="848ec-139">failedCount</span><span class="sxs-lookup"><span data-stu-id="848ec-139">failedCount</span></span>|<span data-ttu-id="848ec-140">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-140">Int32</span></span>|<span data-ttu-id="848ec-141">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="848ec-141">Number of failed devices</span></span>|
|<span data-ttu-id="848ec-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="848ec-142">conflictCount</span></span>|<span data-ttu-id="848ec-143">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-143">Int32</span></span>|<span data-ttu-id="848ec-144">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="848ec-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="848ec-145">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="848ec-145">lastUpdateDateTime</span></span>|<span data-ttu-id="848ec-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="848ec-146">DateTimeOffset</span></span>|<span data-ttu-id="848ec-147">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="848ec-147">Last update time</span></span>|
|<span data-ttu-id="848ec-148">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="848ec-148">configurationVersion</span></span>|<span data-ttu-id="848ec-149">Int32</span><span class="sxs-lookup"><span data-stu-id="848ec-149">Int32</span></span>|<span data-ttu-id="848ec-150">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="848ec-150">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="848ec-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="848ec-151">Relationships</span></span>
<span data-ttu-id="848ec-152">Нет</span><span class="sxs-lookup"><span data-stu-id="848ec-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="848ec-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="848ec-153">JSON Representation</span></span>
<span data-ttu-id="848ec-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="848ec-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





