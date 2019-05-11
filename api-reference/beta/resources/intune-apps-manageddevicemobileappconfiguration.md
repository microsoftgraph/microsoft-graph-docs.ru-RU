---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a532c39a38ea033a3ed1675183528432e4e87211
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950160"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="a7920-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7920-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="a7920-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7920-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7920-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7920-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7920-106">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="a7920-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="a7920-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a7920-107">Methods</span></span>
|<span data-ttu-id="a7920-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a7920-108">Method</span></span>|<span data-ttu-id="a7920-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7920-109">Return Type</span></span>|<span data-ttu-id="a7920-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7920-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7920-111">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="a7920-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="a7920-112">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7920-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="a7920-113">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7920-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a7920-114">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7920-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="a7920-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7920-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="a7920-116">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7920-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a7920-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="a7920-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="a7920-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a7920-118">None</span></span>|<span data-ttu-id="a7920-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a7920-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a7920-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7920-120">Properties</span></span>
|<span data-ttu-id="a7920-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7920-121">Property</span></span>|<span data-ttu-id="a7920-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a7920-122">Type</span></span>|<span data-ttu-id="a7920-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a7920-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7920-124">id</span><span class="sxs-lookup"><span data-stu-id="a7920-124">id</span></span>|<span data-ttu-id="a7920-125">String</span><span class="sxs-lookup"><span data-stu-id="a7920-125">String</span></span>|<span data-ttu-id="a7920-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7920-126">Key of the entity.</span></span>|
|<span data-ttu-id="a7920-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a7920-127">targetedMobileApps</span></span>|<span data-ttu-id="a7920-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7920-128">String collection</span></span>|<span data-ttu-id="a7920-129">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="a7920-129">the associated app.</span></span>|
|<span data-ttu-id="a7920-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7920-130">roleScopeTagIds</span></span>|<span data-ttu-id="a7920-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a7920-131">String collection</span></span>|<span data-ttu-id="a7920-132">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a7920-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="a7920-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7920-133">createdDateTime</span></span>|<span data-ttu-id="a7920-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7920-134">DateTimeOffset</span></span>|<span data-ttu-id="a7920-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a7920-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="a7920-136">description</span><span class="sxs-lookup"><span data-stu-id="a7920-136">description</span></span>|<span data-ttu-id="a7920-137">String</span><span class="sxs-lookup"><span data-stu-id="a7920-137">String</span></span>|<span data-ttu-id="a7920-138">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7920-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a7920-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7920-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a7920-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7920-140">DateTimeOffset</span></span>|<span data-ttu-id="a7920-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a7920-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a7920-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a7920-142">displayName</span></span>|<span data-ttu-id="a7920-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a7920-143">String</span></span>|<span data-ttu-id="a7920-144">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7920-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a7920-145">version</span><span class="sxs-lookup"><span data-stu-id="a7920-145">version</span></span>|<span data-ttu-id="a7920-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a7920-146">Int32</span></span>|<span data-ttu-id="a7920-147">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7920-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7920-148">Связи</span><span class="sxs-lookup"><span data-stu-id="a7920-148">Relationships</span></span>
|<span data-ttu-id="a7920-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="a7920-149">Relationship</span></span>|<span data-ttu-id="a7920-150">Тип</span><span class="sxs-lookup"><span data-stu-id="a7920-150">Type</span></span>|<span data-ttu-id="a7920-151">Описание</span><span class="sxs-lookup"><span data-stu-id="a7920-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7920-152">assignments</span><span class="sxs-lookup"><span data-stu-id="a7920-152">assignments</span></span>|<span data-ttu-id="a7920-153">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7920-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a7920-154">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="a7920-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="a7920-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a7920-155">deviceStatuses</span></span>|<span data-ttu-id="a7920-156">Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="a7920-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a7920-157">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="a7920-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="a7920-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a7920-158">userStatuses</span></span>|<span data-ttu-id="a7920-159">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a7920-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a7920-160">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="a7920-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="a7920-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a7920-161">deviceStatusSummary</span></span>|[<span data-ttu-id="a7920-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="a7920-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="a7920-163">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="a7920-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="a7920-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="a7920-164">userStatusSummary</span></span>|[<span data-ttu-id="a7920-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="a7920-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="a7920-166">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="a7920-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7920-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7920-167">JSON Representation</span></span>
<span data-ttu-id="a7920-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7920-168">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




