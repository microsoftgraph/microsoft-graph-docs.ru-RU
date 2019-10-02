---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f27d69a4cae2ee3a723ea14e4394bc18ba778a8c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359539"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="8ae98-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae98-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="8ae98-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ae98-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae98-105">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="8ae98-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8ae98-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8ae98-106">Methods</span></span>
|<span data-ttu-id="8ae98-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8ae98-107">Method</span></span>|<span data-ttu-id="8ae98-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ae98-108">Return Type</span></span>|<span data-ttu-id="8ae98-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae98-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ae98-110">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae98-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="8ae98-111">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="8ae98-112">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae98-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8ae98-113">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae98-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="8ae98-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae98-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="8ae98-115">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae98-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8ae98-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="8ae98-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="8ae98-117">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ae98-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8ae98-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8ae98-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ae98-119">Properties</span></span>
|<span data-ttu-id="8ae98-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ae98-120">Property</span></span>|<span data-ttu-id="8ae98-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8ae98-121">Type</span></span>|<span data-ttu-id="8ae98-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae98-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae98-123">id</span><span class="sxs-lookup"><span data-stu-id="8ae98-123">id</span></span>|<span data-ttu-id="8ae98-124">String</span><span class="sxs-lookup"><span data-stu-id="8ae98-124">String</span></span>|<span data-ttu-id="8ae98-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae98-125">Key of the entity.</span></span>|
|<span data-ttu-id="8ae98-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae98-126">lastModifiedDateTime</span></span>|<span data-ttu-id="8ae98-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae98-127">DateTimeOffset</span></span>|<span data-ttu-id="8ae98-128">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae98-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8ae98-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae98-129">createdDateTime</span></span>|<span data-ttu-id="8ae98-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae98-130">DateTimeOffset</span></span>|<span data-ttu-id="8ae98-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae98-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="8ae98-132">description</span><span class="sxs-lookup"><span data-stu-id="8ae98-132">description</span></span>|<span data-ttu-id="8ae98-133">String</span><span class="sxs-lookup"><span data-stu-id="8ae98-133">String</span></span>|<span data-ttu-id="8ae98-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae98-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8ae98-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8ae98-135">displayName</span></span>|<span data-ttu-id="8ae98-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8ae98-136">String</span></span>|<span data-ttu-id="8ae98-137">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae98-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8ae98-138">version</span><span class="sxs-lookup"><span data-stu-id="8ae98-138">version</span></span>|<span data-ttu-id="8ae98-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae98-139">Int32</span></span>|<span data-ttu-id="8ae98-140">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae98-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ae98-141">Связи</span><span class="sxs-lookup"><span data-stu-id="8ae98-141">Relationships</span></span>
|<span data-ttu-id="8ae98-142">Связь</span><span class="sxs-lookup"><span data-stu-id="8ae98-142">Relationship</span></span>|<span data-ttu-id="8ae98-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8ae98-143">Type</span></span>|<span data-ttu-id="8ae98-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae98-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae98-145">assignments</span><span class="sxs-lookup"><span data-stu-id="8ae98-145">assignments</span></span>|<span data-ttu-id="8ae98-146">Коллекция объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8ae98-147">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae98-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="8ae98-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8ae98-148">deviceStatuses</span></span>|<span data-ttu-id="8ae98-149">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8ae98-150">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae98-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="8ae98-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8ae98-151">userStatuses</span></span>|<span data-ttu-id="8ae98-152">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8ae98-153">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ae98-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="8ae98-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8ae98-154">deviceStatusOverview</span></span>|[<span data-ttu-id="8ae98-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8ae98-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8ae98-156">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="8ae98-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="8ae98-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8ae98-157">userStatusOverview</span></span>|[<span data-ttu-id="8ae98-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8ae98-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8ae98-159">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="8ae98-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="8ae98-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8ae98-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8ae98-161">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="8ae98-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8ae98-162">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="8ae98-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ae98-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ae98-163">JSON Representation</span></span>
<span data-ttu-id="8ae98-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ae98-164">Here is a JSON representation of the resource.</span></span>
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




