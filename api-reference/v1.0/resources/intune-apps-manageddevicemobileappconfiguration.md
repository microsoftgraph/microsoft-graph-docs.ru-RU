---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 462533c75ebbad87409032c1769edc3d399fda4d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756045"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="980d2-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="980d2-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="980d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="980d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="980d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="980d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="980d2-106">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="980d2-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="980d2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="980d2-107">Methods</span></span>
|<span data-ttu-id="980d2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="980d2-108">Method</span></span>|<span data-ttu-id="980d2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="980d2-109">Return Type</span></span>|<span data-ttu-id="980d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="980d2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="980d2-111">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="980d2-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="980d2-112">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="980d2-113">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="980d2-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="980d2-114">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="980d2-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="980d2-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="980d2-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="980d2-116">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="980d2-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="980d2-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="980d2-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="980d2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="980d2-118">None</span></span>|<span data-ttu-id="980d2-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="980d2-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="980d2-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="980d2-120">Properties</span></span>
|<span data-ttu-id="980d2-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="980d2-121">Property</span></span>|<span data-ttu-id="980d2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="980d2-122">Type</span></span>|<span data-ttu-id="980d2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="980d2-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="980d2-124">id</span><span class="sxs-lookup"><span data-stu-id="980d2-124">id</span></span>|<span data-ttu-id="980d2-125">String</span><span class="sxs-lookup"><span data-stu-id="980d2-125">String</span></span>|<span data-ttu-id="980d2-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="980d2-126">Key of the entity.</span></span>|
|<span data-ttu-id="980d2-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="980d2-127">targetedMobileApps</span></span>|<span data-ttu-id="980d2-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="980d2-128">String collection</span></span>|<span data-ttu-id="980d2-129">Связанное приложение.</span><span class="sxs-lookup"><span data-stu-id="980d2-129">the associated app.</span></span>|
|<span data-ttu-id="980d2-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="980d2-130">createdDateTime</span></span>|<span data-ttu-id="980d2-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980d2-131">DateTimeOffset</span></span>|<span data-ttu-id="980d2-132">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="980d2-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="980d2-133">description</span><span class="sxs-lookup"><span data-stu-id="980d2-133">description</span></span>|<span data-ttu-id="980d2-134">String</span><span class="sxs-lookup"><span data-stu-id="980d2-134">String</span></span>|<span data-ttu-id="980d2-135">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="980d2-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="980d2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="980d2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="980d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980d2-137">DateTimeOffset</span></span>|<span data-ttu-id="980d2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="980d2-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="980d2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="980d2-139">displayName</span></span>|<span data-ttu-id="980d2-140">String</span><span class="sxs-lookup"><span data-stu-id="980d2-140">String</span></span>|<span data-ttu-id="980d2-141">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="980d2-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="980d2-142">version</span><span class="sxs-lookup"><span data-stu-id="980d2-142">version</span></span>|<span data-ttu-id="980d2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="980d2-143">Int32</span></span>|<span data-ttu-id="980d2-144">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="980d2-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="980d2-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="980d2-145">Relationships</span></span>
|<span data-ttu-id="980d2-146">Связь</span><span class="sxs-lookup"><span data-stu-id="980d2-146">Relationship</span></span>|<span data-ttu-id="980d2-147">Тип</span><span class="sxs-lookup"><span data-stu-id="980d2-147">Type</span></span>|<span data-ttu-id="980d2-148">Описание</span><span class="sxs-lookup"><span data-stu-id="980d2-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="980d2-149">assignments</span><span class="sxs-lookup"><span data-stu-id="980d2-149">assignments</span></span>|<span data-ttu-id="980d2-150">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="980d2-151">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="980d2-151">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="980d2-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="980d2-152">deviceStatuses</span></span>|<span data-ttu-id="980d2-153">[коллекция managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="980d2-154">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="980d2-154">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="980d2-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="980d2-155">userStatuses</span></span>|<span data-ttu-id="980d2-156">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="980d2-157">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="980d2-157">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="980d2-158">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="980d2-158">deviceStatusSummary</span></span>|[<span data-ttu-id="980d2-159">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="980d2-159">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="980d2-160">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="980d2-160">App configuration device status summary.</span></span>|
|<span data-ttu-id="980d2-161">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="980d2-161">userStatusSummary</span></span>|[<span data-ttu-id="980d2-162">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="980d2-162">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="980d2-163">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="980d2-163">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="980d2-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="980d2-164">JSON Representation</span></span>
<span data-ttu-id="980d2-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="980d2-165">Here is a JSON representation of the resource.</span></span>
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




