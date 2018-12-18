---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: tfitzmac
ms.openlocfilehash: c51db6ddad8b23957da9ed9b8d132c416e52f073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360027"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="f4143-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4143-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="f4143-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4143-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4143-105">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="f4143-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="f4143-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f4143-106">Methods</span></span>
|<span data-ttu-id="f4143-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f4143-107">Method</span></span>|<span data-ttu-id="f4143-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4143-108">Return Type</span></span>|<span data-ttu-id="f4143-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f4143-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4143-110">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="f4143-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="f4143-111">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4143-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="f4143-112">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4143-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f4143-113">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4143-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="f4143-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4143-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="f4143-115">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4143-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f4143-116">Действие assign</span><span class="sxs-lookup"><span data-stu-id="f4143-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="f4143-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f4143-117">None</span></span>|<span data-ttu-id="f4143-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f4143-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f4143-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4143-119">Properties</span></span>
|<span data-ttu-id="f4143-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4143-120">Property</span></span>|<span data-ttu-id="f4143-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f4143-121">Type</span></span>|<span data-ttu-id="f4143-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f4143-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4143-123">id</span><span class="sxs-lookup"><span data-stu-id="f4143-123">id</span></span>|<span data-ttu-id="f4143-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f4143-124">String</span></span>|<span data-ttu-id="f4143-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4143-125">Key of the entity.</span></span>|
|<span data-ttu-id="f4143-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f4143-126">targetedMobileApps</span></span>|<span data-ttu-id="f4143-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f4143-127">String collection</span></span>|<span data-ttu-id="f4143-128">Связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="f4143-128">the associated app.</span></span>|
|<span data-ttu-id="f4143-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4143-129">createdDateTime</span></span>|<span data-ttu-id="f4143-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4143-130">DateTimeOffset</span></span>|<span data-ttu-id="f4143-131">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f4143-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="f4143-132">описание</span><span class="sxs-lookup"><span data-stu-id="f4143-132">description</span></span>|<span data-ttu-id="f4143-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f4143-133">String</span></span>|<span data-ttu-id="f4143-134">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4143-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f4143-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4143-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f4143-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4143-136">DateTimeOffset</span></span>|<span data-ttu-id="f4143-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f4143-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f4143-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f4143-138">displayName</span></span>|<span data-ttu-id="f4143-139">Строка</span><span class="sxs-lookup"><span data-stu-id="f4143-139">String</span></span>|<span data-ttu-id="f4143-140">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4143-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f4143-141">version</span><span class="sxs-lookup"><span data-stu-id="f4143-141">version</span></span>|<span data-ttu-id="f4143-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f4143-142">Int32</span></span>|<span data-ttu-id="f4143-143">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4143-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4143-144">Связи</span><span class="sxs-lookup"><span data-stu-id="f4143-144">Relationships</span></span>
|<span data-ttu-id="f4143-145">Связь</span><span class="sxs-lookup"><span data-stu-id="f4143-145">Relationship</span></span>|<span data-ttu-id="f4143-146">Тип</span><span class="sxs-lookup"><span data-stu-id="f4143-146">Type</span></span>|<span data-ttu-id="f4143-147">Описание</span><span class="sxs-lookup"><span data-stu-id="f4143-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4143-148">assignments</span><span class="sxs-lookup"><span data-stu-id="f4143-148">assignments</span></span>|<span data-ttu-id="f4143-149">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f4143-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f4143-150">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="f4143-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="f4143-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f4143-151">deviceStatuses</span></span>|<span data-ttu-id="f4143-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f4143-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="f4143-153">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="f4143-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="f4143-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f4143-154">userStatuses</span></span>|<span data-ttu-id="f4143-155">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f4143-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="f4143-156">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="f4143-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="f4143-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="f4143-157">deviceStatusSummary</span></span>|[<span data-ttu-id="f4143-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="f4143-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="f4143-159">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="f4143-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="f4143-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="f4143-160">userStatusSummary</span></span>|[<span data-ttu-id="f4143-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f4143-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="f4143-162">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="f4143-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4143-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4143-163">JSON Representation</span></span>
<span data-ttu-id="f4143-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4143-164">Here is a JSON representation of the resource.</span></span>
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



