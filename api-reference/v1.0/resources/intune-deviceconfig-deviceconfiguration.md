---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a3d0ecc27fc0fe29ed2ed3ca4080e3fea70d264
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560790"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="cf299-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf299-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="cf299-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf299-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf299-105">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="cf299-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="cf299-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cf299-106">Methods</span></span>
|<span data-ttu-id="cf299-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cf299-107">Method</span></span>|<span data-ttu-id="cf299-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf299-108">Return Type</span></span>|<span data-ttu-id="cf299-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf299-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf299-110">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf299-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="cf299-111">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="cf299-112">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf299-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cf299-113">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf299-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="cf299-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf299-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="cf299-115">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf299-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="cf299-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="cf299-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="cf299-117">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cf299-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cf299-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cf299-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf299-119">Properties</span></span>
|<span data-ttu-id="cf299-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf299-120">Property</span></span>|<span data-ttu-id="cf299-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cf299-121">Type</span></span>|<span data-ttu-id="cf299-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cf299-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf299-123">id</span><span class="sxs-lookup"><span data-stu-id="cf299-123">id</span></span>|<span data-ttu-id="cf299-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cf299-124">String</span></span>|<span data-ttu-id="cf299-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf299-125">Key of the entity.</span></span>|
|<span data-ttu-id="cf299-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf299-126">lastModifiedDateTime</span></span>|<span data-ttu-id="cf299-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf299-127">DateTimeOffset</span></span>|<span data-ttu-id="cf299-128">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cf299-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="cf299-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf299-129">createdDateTime</span></span>|<span data-ttu-id="cf299-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf299-130">DateTimeOffset</span></span>|<span data-ttu-id="cf299-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cf299-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="cf299-132">description</span><span class="sxs-lookup"><span data-stu-id="cf299-132">description</span></span>|<span data-ttu-id="cf299-133">String</span><span class="sxs-lookup"><span data-stu-id="cf299-133">String</span></span>|<span data-ttu-id="cf299-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf299-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="cf299-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cf299-135">displayName</span></span>|<span data-ttu-id="cf299-136">String</span><span class="sxs-lookup"><span data-stu-id="cf299-136">String</span></span>|<span data-ttu-id="cf299-137">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf299-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="cf299-138">version</span><span class="sxs-lookup"><span data-stu-id="cf299-138">version</span></span>|<span data-ttu-id="cf299-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cf299-139">Int32</span></span>|<span data-ttu-id="cf299-140">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf299-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf299-141">Связи</span><span class="sxs-lookup"><span data-stu-id="cf299-141">Relationships</span></span>
|<span data-ttu-id="cf299-142">Отношение</span><span class="sxs-lookup"><span data-stu-id="cf299-142">Relationship</span></span>|<span data-ttu-id="cf299-143">Тип</span><span class="sxs-lookup"><span data-stu-id="cf299-143">Type</span></span>|<span data-ttu-id="cf299-144">Описание</span><span class="sxs-lookup"><span data-stu-id="cf299-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf299-145">assignments</span><span class="sxs-lookup"><span data-stu-id="cf299-145">assignments</span></span>|<span data-ttu-id="cf299-146">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cf299-147">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf299-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="cf299-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="cf299-148">deviceStatuses</span></span>|<span data-ttu-id="cf299-149">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="cf299-150">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="cf299-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="cf299-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="cf299-151">userStatuses</span></span>|<span data-ttu-id="cf299-152">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="cf299-153">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="cf299-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="cf299-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="cf299-154">deviceStatusOverview</span></span>|[<span data-ttu-id="cf299-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cf299-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="cf299-156">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="cf299-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="cf299-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="cf299-157">userStatusOverview</span></span>|[<span data-ttu-id="cf299-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="cf299-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="cf299-159">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="cf299-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="cf299-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="cf299-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="cf299-161">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="cf299-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="cf299-162">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="cf299-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf299-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf299-163">JSON Representation</span></span>
<span data-ttu-id="cf299-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf299-164">Here is a JSON representation of the resource.</span></span>
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



