---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a508a037dbd1271d30a226d9cf62fb0683b53af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953149"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="8eb49-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eb49-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="8eb49-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8eb49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8eb49-105">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="8eb49-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="8eb49-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8eb49-106">Methods</span></span>
|<span data-ttu-id="8eb49-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8eb49-107">Method</span></span>|<span data-ttu-id="8eb49-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8eb49-108">Return Type</span></span>|<span data-ttu-id="8eb49-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb49-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8eb49-110">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eb49-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="8eb49-111">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="8eb49-112">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb49-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8eb49-113">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eb49-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="8eb49-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8eb49-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="8eb49-115">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8eb49-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8eb49-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="8eb49-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="8eb49-117">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8eb49-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8eb49-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8eb49-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8eb49-119">Properties</span></span>
|<span data-ttu-id="8eb49-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8eb49-120">Property</span></span>|<span data-ttu-id="8eb49-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb49-121">Type</span></span>|<span data-ttu-id="8eb49-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb49-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb49-123">id</span><span class="sxs-lookup"><span data-stu-id="8eb49-123">id</span></span>|<span data-ttu-id="8eb49-124">String</span><span class="sxs-lookup"><span data-stu-id="8eb49-124">String</span></span>|<span data-ttu-id="8eb49-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb49-125">Key of the entity.</span></span>|
|<span data-ttu-id="8eb49-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb49-126">lastModifiedDateTime</span></span>|<span data-ttu-id="8eb49-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb49-127">DateTimeOffset</span></span>|<span data-ttu-id="8eb49-128">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb49-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8eb49-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb49-129">createdDateTime</span></span>|<span data-ttu-id="8eb49-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb49-130">DateTimeOffset</span></span>|<span data-ttu-id="8eb49-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8eb49-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="8eb49-132">описание</span><span class="sxs-lookup"><span data-stu-id="8eb49-132">description</span></span>|<span data-ttu-id="8eb49-133">String</span><span class="sxs-lookup"><span data-stu-id="8eb49-133">String</span></span>|<span data-ttu-id="8eb49-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb49-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8eb49-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb49-135">displayName</span></span>|<span data-ttu-id="8eb49-136">String</span><span class="sxs-lookup"><span data-stu-id="8eb49-136">String</span></span>|<span data-ttu-id="8eb49-137">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb49-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8eb49-138">version</span><span class="sxs-lookup"><span data-stu-id="8eb49-138">version</span></span>|<span data-ttu-id="8eb49-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8eb49-139">Int32</span></span>|<span data-ttu-id="8eb49-140">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb49-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eb49-141">Связи</span><span class="sxs-lookup"><span data-stu-id="8eb49-141">Relationships</span></span>
|<span data-ttu-id="8eb49-142">Связь</span><span class="sxs-lookup"><span data-stu-id="8eb49-142">Relationship</span></span>|<span data-ttu-id="8eb49-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb49-143">Type</span></span>|<span data-ttu-id="8eb49-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb49-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb49-145">assignments</span><span class="sxs-lookup"><span data-stu-id="8eb49-145">assignments</span></span>|<span data-ttu-id="8eb49-146">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8eb49-147">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb49-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="8eb49-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8eb49-148">deviceStatuses</span></span>|<span data-ttu-id="8eb49-149">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8eb49-150">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="8eb49-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="8eb49-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8eb49-151">userStatuses</span></span>|<span data-ttu-id="8eb49-152">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8eb49-153">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="8eb49-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="8eb49-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8eb49-154">deviceStatusOverview</span></span>|[<span data-ttu-id="8eb49-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8eb49-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8eb49-156">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="8eb49-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="8eb49-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8eb49-157">userStatusOverview</span></span>|[<span data-ttu-id="8eb49-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8eb49-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8eb49-159">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="8eb49-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="8eb49-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8eb49-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8eb49-161">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="8eb49-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8eb49-162">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="8eb49-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8eb49-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8eb49-163">JSON Representation</span></span>
<span data-ttu-id="8eb49-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8eb49-164">Here is a JSON representation of the resource.</span></span>
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



