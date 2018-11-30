---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
ms.openlocfilehash: 7cde579aa9d2e096380286d628a9964d4522f402
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028524"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="3399f-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3399f-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="3399f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3399f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3399f-105">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="3399f-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="3399f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3399f-106">Methods</span></span>
|<span data-ttu-id="3399f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3399f-107">Method</span></span>|<span data-ttu-id="3399f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3399f-108">Return Type</span></span>|<span data-ttu-id="3399f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3399f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3399f-110">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3399f-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="3399f-111">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="3399f-112">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3399f-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3399f-113">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3399f-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="3399f-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3399f-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="3399f-115">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3399f-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3399f-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="3399f-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="3399f-117">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3399f-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3399f-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3399f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3399f-119">Properties</span></span>
|<span data-ttu-id="3399f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3399f-120">Property</span></span>|<span data-ttu-id="3399f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3399f-121">Type</span></span>|<span data-ttu-id="3399f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3399f-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3399f-123">id</span><span class="sxs-lookup"><span data-stu-id="3399f-123">id</span></span>|<span data-ttu-id="3399f-124">String</span><span class="sxs-lookup"><span data-stu-id="3399f-124">String</span></span>|<span data-ttu-id="3399f-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3399f-125">Key of the entity.</span></span>|
|<span data-ttu-id="3399f-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3399f-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3399f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3399f-127">DateTimeOffset</span></span>|<span data-ttu-id="3399f-128">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3399f-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3399f-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3399f-129">createdDateTime</span></span>|<span data-ttu-id="3399f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3399f-130">DateTimeOffset</span></span>|<span data-ttu-id="3399f-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3399f-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="3399f-132">описание</span><span class="sxs-lookup"><span data-stu-id="3399f-132">description</span></span>|<span data-ttu-id="3399f-133">String</span><span class="sxs-lookup"><span data-stu-id="3399f-133">String</span></span>|<span data-ttu-id="3399f-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3399f-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3399f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3399f-135">displayName</span></span>|<span data-ttu-id="3399f-136">String</span><span class="sxs-lookup"><span data-stu-id="3399f-136">String</span></span>|<span data-ttu-id="3399f-137">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3399f-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3399f-138">version</span><span class="sxs-lookup"><span data-stu-id="3399f-138">version</span></span>|<span data-ttu-id="3399f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3399f-139">Int32</span></span>|<span data-ttu-id="3399f-140">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3399f-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3399f-141">Связи</span><span class="sxs-lookup"><span data-stu-id="3399f-141">Relationships</span></span>
|<span data-ttu-id="3399f-142">Связь</span><span class="sxs-lookup"><span data-stu-id="3399f-142">Relationship</span></span>|<span data-ttu-id="3399f-143">Тип</span><span class="sxs-lookup"><span data-stu-id="3399f-143">Type</span></span>|<span data-ttu-id="3399f-144">Описание</span><span class="sxs-lookup"><span data-stu-id="3399f-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3399f-145">assignments</span><span class="sxs-lookup"><span data-stu-id="3399f-145">assignments</span></span>|<span data-ttu-id="3399f-146">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3399f-147">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3399f-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="3399f-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3399f-148">deviceStatuses</span></span>|<span data-ttu-id="3399f-149">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3399f-150">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="3399f-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="3399f-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3399f-151">userStatuses</span></span>|<span data-ttu-id="3399f-152">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3399f-153">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="3399f-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="3399f-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3399f-154">deviceStatusOverview</span></span>|[<span data-ttu-id="3399f-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3399f-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3399f-156">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="3399f-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="3399f-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3399f-157">userStatusOverview</span></span>|[<span data-ttu-id="3399f-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3399f-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3399f-159">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="3399f-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="3399f-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3399f-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3399f-161">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3399f-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3399f-162">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="3399f-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3399f-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3399f-163">JSON Representation</span></span>
<span data-ttu-id="3399f-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3399f-164">Here is a JSON representation of the resource.</span></span>
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



