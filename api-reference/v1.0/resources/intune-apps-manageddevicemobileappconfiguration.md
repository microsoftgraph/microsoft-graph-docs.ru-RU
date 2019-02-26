---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1a249325f7e4c9be196c5adda695b84e5f8a94c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258599"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="1e0bf-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e0bf-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="1e0bf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e0bf-105">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="1e0bf-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1e0bf-106">Methods</span></span>
|<span data-ttu-id="1e0bf-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1e0bf-107">Method</span></span>|<span data-ttu-id="1e0bf-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e0bf-108">Return Type</span></span>|<span data-ttu-id="1e0bf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0bf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e0bf-110">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="1e0bf-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="1e0bf-111">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="1e0bf-112">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0bf-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1e0bf-113">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e0bf-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="1e0bf-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e0bf-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="1e0bf-115">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1e0bf-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1e0bf-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="1e0bf-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="1e0bf-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1e0bf-117">None</span></span>|<span data-ttu-id="1e0bf-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1e0bf-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1e0bf-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e0bf-119">Properties</span></span>
|<span data-ttu-id="1e0bf-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e0bf-120">Property</span></span>|<span data-ttu-id="1e0bf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1e0bf-121">Type</span></span>|<span data-ttu-id="1e0bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0bf-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0bf-123">id</span><span class="sxs-lookup"><span data-stu-id="1e0bf-123">id</span></span>|<span data-ttu-id="1e0bf-124">String</span><span class="sxs-lookup"><span data-stu-id="1e0bf-124">String</span></span>|<span data-ttu-id="1e0bf-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-125">Key of the entity.</span></span>|
|<span data-ttu-id="1e0bf-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1e0bf-126">targetedMobileApps</span></span>|<span data-ttu-id="1e0bf-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e0bf-127">String collection</span></span>|<span data-ttu-id="1e0bf-128">Связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-128">the associated app.</span></span>|
|<span data-ttu-id="1e0bf-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0bf-129">createdDateTime</span></span>|<span data-ttu-id="1e0bf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0bf-130">DateTimeOffset</span></span>|<span data-ttu-id="1e0bf-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="1e0bf-132">description</span><span class="sxs-lookup"><span data-stu-id="1e0bf-132">description</span></span>|<span data-ttu-id="1e0bf-133">String</span><span class="sxs-lookup"><span data-stu-id="1e0bf-133">String</span></span>|<span data-ttu-id="1e0bf-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="1e0bf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e0bf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1e0bf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e0bf-136">DateTimeOffset</span></span>|<span data-ttu-id="1e0bf-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1e0bf-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1e0bf-138">displayName</span></span>|<span data-ttu-id="1e0bf-139">String</span><span class="sxs-lookup"><span data-stu-id="1e0bf-139">String</span></span>|<span data-ttu-id="1e0bf-140">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="1e0bf-141">version</span><span class="sxs-lookup"><span data-stu-id="1e0bf-141">version</span></span>|<span data-ttu-id="1e0bf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1e0bf-142">Int32</span></span>|<span data-ttu-id="1e0bf-143">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e0bf-144">Связи</span><span class="sxs-lookup"><span data-stu-id="1e0bf-144">Relationships</span></span>
|<span data-ttu-id="1e0bf-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="1e0bf-145">Relationship</span></span>|<span data-ttu-id="1e0bf-146">Тип</span><span class="sxs-lookup"><span data-stu-id="1e0bf-146">Type</span></span>|<span data-ttu-id="1e0bf-147">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0bf-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e0bf-148">assignments</span><span class="sxs-lookup"><span data-stu-id="1e0bf-148">assignments</span></span>|<span data-ttu-id="1e0bf-149">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1e0bf-150">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="1e0bf-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1e0bf-151">deviceStatuses</span></span>|<span data-ttu-id="1e0bf-152">Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1e0bf-153">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="1e0bf-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1e0bf-154">userStatuses</span></span>|<span data-ttu-id="1e0bf-155">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1e0bf-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1e0bf-156">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="1e0bf-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="1e0bf-157">deviceStatusSummary</span></span>|[<span data-ttu-id="1e0bf-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1e0bf-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="1e0bf-159">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="1e0bf-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="1e0bf-160">userStatusSummary</span></span>|[<span data-ttu-id="1e0bf-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="1e0bf-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="1e0bf-162">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e0bf-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e0bf-163">JSON Representation</span></span>
<span data-ttu-id="1e0bf-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e0bf-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



