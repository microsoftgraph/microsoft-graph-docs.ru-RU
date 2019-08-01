---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a833936d24594159708d7dfe3fc8a451d0893e98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029052"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="43cf0-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="43cf0-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="43cf0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43cf0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43cf0-105">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="43cf0-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="43cf0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="43cf0-106">Methods</span></span>
|<span data-ttu-id="43cf0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="43cf0-107">Method</span></span>|<span data-ttu-id="43cf0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="43cf0-108">Return Type</span></span>|<span data-ttu-id="43cf0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="43cf0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43cf0-110">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="43cf0-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="43cf0-111">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43cf0-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="43cf0-112">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43cf0-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="43cf0-113">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="43cf0-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="43cf0-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="43cf0-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="43cf0-115">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43cf0-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="43cf0-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="43cf0-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="43cf0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="43cf0-117">None</span></span>|<span data-ttu-id="43cf0-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="43cf0-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="43cf0-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="43cf0-119">Properties</span></span>
|<span data-ttu-id="43cf0-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="43cf0-120">Property</span></span>|<span data-ttu-id="43cf0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="43cf0-121">Type</span></span>|<span data-ttu-id="43cf0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43cf0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cf0-123">id</span><span class="sxs-lookup"><span data-stu-id="43cf0-123">id</span></span>|<span data-ttu-id="43cf0-124">String</span><span class="sxs-lookup"><span data-stu-id="43cf0-124">String</span></span>|<span data-ttu-id="43cf0-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="43cf0-125">Key of the entity.</span></span>|
|<span data-ttu-id="43cf0-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="43cf0-126">targetedMobileApps</span></span>|<span data-ttu-id="43cf0-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="43cf0-127">String collection</span></span>|<span data-ttu-id="43cf0-128">Связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="43cf0-128">the associated app.</span></span>|
|<span data-ttu-id="43cf0-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43cf0-129">createdDateTime</span></span>|<span data-ttu-id="43cf0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cf0-130">DateTimeOffset</span></span>|<span data-ttu-id="43cf0-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="43cf0-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="43cf0-132">description</span><span class="sxs-lookup"><span data-stu-id="43cf0-132">description</span></span>|<span data-ttu-id="43cf0-133">String</span><span class="sxs-lookup"><span data-stu-id="43cf0-133">String</span></span>|<span data-ttu-id="43cf0-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43cf0-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="43cf0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43cf0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="43cf0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43cf0-136">DateTimeOffset</span></span>|<span data-ttu-id="43cf0-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="43cf0-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="43cf0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="43cf0-138">displayName</span></span>|<span data-ttu-id="43cf0-139">Строка</span><span class="sxs-lookup"><span data-stu-id="43cf0-139">String</span></span>|<span data-ttu-id="43cf0-140">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43cf0-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="43cf0-141">version</span><span class="sxs-lookup"><span data-stu-id="43cf0-141">version</span></span>|<span data-ttu-id="43cf0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="43cf0-142">Int32</span></span>|<span data-ttu-id="43cf0-143">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43cf0-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43cf0-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="43cf0-144">Relationships</span></span>
|<span data-ttu-id="43cf0-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="43cf0-145">Relationship</span></span>|<span data-ttu-id="43cf0-146">Тип</span><span class="sxs-lookup"><span data-stu-id="43cf0-146">Type</span></span>|<span data-ttu-id="43cf0-147">Описание</span><span class="sxs-lookup"><span data-stu-id="43cf0-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43cf0-148">assignments</span><span class="sxs-lookup"><span data-stu-id="43cf0-148">assignments</span></span>|<span data-ttu-id="43cf0-149">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="43cf0-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="43cf0-150">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="43cf0-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="43cf0-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="43cf0-151">deviceStatuses</span></span>|<span data-ttu-id="43cf0-152">Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="43cf0-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="43cf0-153">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="43cf0-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="43cf0-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="43cf0-154">userStatuses</span></span>|<span data-ttu-id="43cf0-155">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="43cf0-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="43cf0-156">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="43cf0-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="43cf0-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="43cf0-157">deviceStatusSummary</span></span>|[<span data-ttu-id="43cf0-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="43cf0-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="43cf0-159">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="43cf0-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="43cf0-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="43cf0-160">userStatusSummary</span></span>|[<span data-ttu-id="43cf0-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="43cf0-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="43cf0-162">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="43cf0-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43cf0-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43cf0-163">JSON Representation</span></span>
<span data-ttu-id="43cf0-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43cf0-164">Here is a JSON representation of the resource.</span></span>
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



