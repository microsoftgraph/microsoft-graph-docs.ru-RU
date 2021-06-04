---
title: Тип ресурса deviceConfiguration
description: Конфигурация устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82f1de5e835ceba2a15559411a07638dee2602bd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742911"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="5baba-103">Тип ресурса deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5baba-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="5baba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5baba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5baba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5baba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5baba-106">Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="5baba-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5baba-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5baba-107">Methods</span></span>
|<span data-ttu-id="5baba-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5baba-108">Method</span></span>|<span data-ttu-id="5baba-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5baba-109">Return Type</span></span>|<span data-ttu-id="5baba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5baba-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5baba-111">Список объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5baba-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="5baba-112">Коллекция [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="5baba-113">Список свойств и связей объектов [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5baba-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="5baba-114">Получение объекта deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5baba-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="5baba-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5baba-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="5baba-116">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5baba-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="5baba-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="5baba-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="5baba-118">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5baba-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5baba-119">Not yet documented</span></span>|
|[<span data-ttu-id="5baba-120">функция getOmaSettingPlainTextValue</span><span class="sxs-lookup"><span data-stu-id="5baba-120">getOmaSettingPlainTextValue function</span></span>](../api/intune-deviceconfig-deviceconfiguration-getomasettingplaintextvalue.md)|<span data-ttu-id="5baba-121">String</span><span class="sxs-lookup"><span data-stu-id="5baba-121">String</span></span>|<span data-ttu-id="5baba-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5baba-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5baba-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="5baba-123">Properties</span></span>
|<span data-ttu-id="5baba-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="5baba-124">Property</span></span>|<span data-ttu-id="5baba-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5baba-125">Type</span></span>|<span data-ttu-id="5baba-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5baba-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5baba-127">id</span><span class="sxs-lookup"><span data-stu-id="5baba-127">id</span></span>|<span data-ttu-id="5baba-128">String</span><span class="sxs-lookup"><span data-stu-id="5baba-128">String</span></span>|<span data-ttu-id="5baba-129">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5baba-129">Key of the entity.</span></span>|
|<span data-ttu-id="5baba-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5baba-130">lastModifiedDateTime</span></span>|<span data-ttu-id="5baba-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5baba-131">DateTimeOffset</span></span>|<span data-ttu-id="5baba-132">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5baba-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5baba-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5baba-133">createdDateTime</span></span>|<span data-ttu-id="5baba-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5baba-134">DateTimeOffset</span></span>|<span data-ttu-id="5baba-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5baba-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="5baba-136">description</span><span class="sxs-lookup"><span data-stu-id="5baba-136">description</span></span>|<span data-ttu-id="5baba-137">String</span><span class="sxs-lookup"><span data-stu-id="5baba-137">String</span></span>|<span data-ttu-id="5baba-138">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5baba-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="5baba-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5baba-139">displayName</span></span>|<span data-ttu-id="5baba-140">String</span><span class="sxs-lookup"><span data-stu-id="5baba-140">String</span></span>|<span data-ttu-id="5baba-141">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5baba-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5baba-142">version</span><span class="sxs-lookup"><span data-stu-id="5baba-142">version</span></span>|<span data-ttu-id="5baba-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5baba-143">Int32</span></span>|<span data-ttu-id="5baba-144">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5baba-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5baba-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="5baba-145">Relationships</span></span>
|<span data-ttu-id="5baba-146">Связь</span><span class="sxs-lookup"><span data-stu-id="5baba-146">Relationship</span></span>|<span data-ttu-id="5baba-147">Тип</span><span class="sxs-lookup"><span data-stu-id="5baba-147">Type</span></span>|<span data-ttu-id="5baba-148">Описание</span><span class="sxs-lookup"><span data-stu-id="5baba-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5baba-149">assignments</span><span class="sxs-lookup"><span data-stu-id="5baba-149">assignments</span></span>|<span data-ttu-id="5baba-150">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-150">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5baba-151">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5baba-151">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="5baba-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5baba-152">deviceStatuses</span></span>|<span data-ttu-id="5baba-153">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-153">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="5baba-154">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="5baba-154">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="5baba-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5baba-155">userStatuses</span></span>|<span data-ttu-id="5baba-156">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-156">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="5baba-157">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="5baba-157">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="5baba-158">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5baba-158">deviceStatusOverview</span></span>|[<span data-ttu-id="5baba-159">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5baba-159">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="5baba-160">Обзор состояния конфигураций устройств</span><span class="sxs-lookup"><span data-stu-id="5baba-160">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="5baba-161">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="5baba-161">userStatusOverview</span></span>|[<span data-ttu-id="5baba-162">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="5baba-162">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="5baba-163">Обзор состояния конфигураций устройств по пользователям</span><span class="sxs-lookup"><span data-stu-id="5baba-163">Device Configuration users status overview</span></span>|
|<span data-ttu-id="5baba-164">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="5baba-164">deviceSettingStateSummaries</span></span>|<span data-ttu-id="5baba-165">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5baba-165">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="5baba-166">Сводка по состоянию параметров конфигурации устройств</span><span class="sxs-lookup"><span data-stu-id="5baba-166">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5baba-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5baba-167">JSON Representation</span></span>
<span data-ttu-id="5baba-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5baba-168">Here is a JSON representation of the resource.</span></span>
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




