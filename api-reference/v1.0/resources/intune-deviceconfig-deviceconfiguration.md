---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1927b4af889fb98e2e9c33561b9ff63042df5b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465743"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="e7766-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7766-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="e7766-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7766-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7766-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7766-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7766-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="e7766-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="e7766-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e7766-107">Methods</span></span>
|<span data-ttu-id="e7766-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e7766-108">Method</span></span>|<span data-ttu-id="e7766-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e7766-109">Return Type</span></span>|<span data-ttu-id="e7766-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e7766-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e7766-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7766-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="e7766-112">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="e7766-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7766-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e7766-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7766-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="e7766-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7766-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="e7766-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7766-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e7766-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e7766-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="e7766-118">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e7766-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7766-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e7766-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7766-120">Properties</span></span>
|<span data-ttu-id="e7766-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7766-121">Property</span></span>|<span data-ttu-id="e7766-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e7766-122">Type</span></span>|<span data-ttu-id="e7766-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e7766-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7766-124">id</span><span class="sxs-lookup"><span data-stu-id="e7766-124">id</span></span>|<span data-ttu-id="e7766-125">String</span><span class="sxs-lookup"><span data-stu-id="e7766-125">String</span></span>|<span data-ttu-id="e7766-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7766-126">Key of the entity.</span></span>|
|<span data-ttu-id="e7766-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7766-127">lastModifiedDateTime</span></span>|<span data-ttu-id="e7766-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7766-128">DateTimeOffset</span></span>|<span data-ttu-id="e7766-129">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e7766-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e7766-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7766-130">createdDateTime</span></span>|<span data-ttu-id="e7766-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7766-131">DateTimeOffset</span></span>|<span data-ttu-id="e7766-132">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e7766-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="e7766-133">description</span><span class="sxs-lookup"><span data-stu-id="e7766-133">description</span></span>|<span data-ttu-id="e7766-134">String</span><span class="sxs-lookup"><span data-stu-id="e7766-134">String</span></span>|<span data-ttu-id="e7766-135">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7766-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="e7766-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e7766-136">displayName</span></span>|<span data-ttu-id="e7766-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e7766-137">String</span></span>|<span data-ttu-id="e7766-138">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7766-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="e7766-139">version</span><span class="sxs-lookup"><span data-stu-id="e7766-139">version</span></span>|<span data-ttu-id="e7766-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e7766-140">Int32</span></span>|<span data-ttu-id="e7766-141">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7766-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7766-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="e7766-142">Relationships</span></span>
|<span data-ttu-id="e7766-143">Связь</span><span class="sxs-lookup"><span data-stu-id="e7766-143">Relationship</span></span>|<span data-ttu-id="e7766-144">Тип</span><span class="sxs-lookup"><span data-stu-id="e7766-144">Type</span></span>|<span data-ttu-id="e7766-145">Описание</span><span class="sxs-lookup"><span data-stu-id="e7766-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7766-146">assignments</span><span class="sxs-lookup"><span data-stu-id="e7766-146">assignments</span></span>|<span data-ttu-id="e7766-147">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e7766-148">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7766-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="e7766-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e7766-149">deviceStatuses</span></span>|<span data-ttu-id="e7766-150">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="e7766-151">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="e7766-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="e7766-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="e7766-152">userStatuses</span></span>|<span data-ttu-id="e7766-153">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="e7766-154">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="e7766-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="e7766-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="e7766-155">deviceStatusOverview</span></span>|[<span data-ttu-id="e7766-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e7766-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="e7766-157">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="e7766-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="e7766-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="e7766-158">userStatusOverview</span></span>|[<span data-ttu-id="e7766-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="e7766-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="e7766-160">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="e7766-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="e7766-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="e7766-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="e7766-162">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e7766-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="e7766-163">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="e7766-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7766-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7766-164">JSON Representation</span></span>
<span data-ttu-id="e7766-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7766-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```







