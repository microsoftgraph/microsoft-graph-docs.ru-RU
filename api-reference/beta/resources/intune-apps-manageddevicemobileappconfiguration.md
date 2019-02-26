---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dacccb00a30028a5b9e5144eb843ca52c60da876
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154252"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="7ef17-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ef17-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="7ef17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ef17-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ef17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ef17-106">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="7ef17-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="7ef17-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7ef17-107">Methods</span></span>
|<span data-ttu-id="7ef17-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7ef17-108">Method</span></span>|<span data-ttu-id="7ef17-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ef17-109">Return Type</span></span>|<span data-ttu-id="7ef17-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef17-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ef17-111">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7ef17-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="7ef17-112">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ef17-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="7ef17-113">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef17-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7ef17-114">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ef17-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="7ef17-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ef17-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="7ef17-116">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef17-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7ef17-117">Действие assign</span><span class="sxs-lookup"><span data-stu-id="7ef17-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="7ef17-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7ef17-118">None</span></span>|<span data-ttu-id="7ef17-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7ef17-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7ef17-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ef17-120">Properties</span></span>
|<span data-ttu-id="7ef17-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ef17-121">Property</span></span>|<span data-ttu-id="7ef17-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef17-122">Type</span></span>|<span data-ttu-id="7ef17-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef17-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef17-124">id</span><span class="sxs-lookup"><span data-stu-id="7ef17-124">id</span></span>|<span data-ttu-id="7ef17-125">String</span><span class="sxs-lookup"><span data-stu-id="7ef17-125">String</span></span>|<span data-ttu-id="7ef17-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef17-126">Key of the entity.</span></span>|
|<span data-ttu-id="7ef17-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7ef17-127">targetedMobileApps</span></span>|<span data-ttu-id="7ef17-128">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7ef17-128">String collection</span></span>|<span data-ttu-id="7ef17-129">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="7ef17-129">the associated app.</span></span>|
|<span data-ttu-id="7ef17-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ef17-130">roleScopeTagIds</span></span>|<span data-ttu-id="7ef17-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7ef17-131">String collection</span></span>|<span data-ttu-id="7ef17-132">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="7ef17-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="7ef17-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef17-133">createdDateTime</span></span>|<span data-ttu-id="7ef17-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef17-134">DateTimeOffset</span></span>|<span data-ttu-id="7ef17-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef17-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="7ef17-136">description</span><span class="sxs-lookup"><span data-stu-id="7ef17-136">description</span></span>|<span data-ttu-id="7ef17-137">String</span><span class="sxs-lookup"><span data-stu-id="7ef17-137">String</span></span>|<span data-ttu-id="7ef17-138">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef17-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7ef17-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef17-139">lastModifiedDateTime</span></span>|<span data-ttu-id="7ef17-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef17-140">DateTimeOffset</span></span>|<span data-ttu-id="7ef17-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7ef17-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7ef17-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7ef17-142">displayName</span></span>|<span data-ttu-id="7ef17-143">String</span><span class="sxs-lookup"><span data-stu-id="7ef17-143">String</span></span>|<span data-ttu-id="7ef17-144">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef17-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7ef17-145">version</span><span class="sxs-lookup"><span data-stu-id="7ef17-145">version</span></span>|<span data-ttu-id="7ef17-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7ef17-146">Int32</span></span>|<span data-ttu-id="7ef17-147">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7ef17-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ef17-148">Связи</span><span class="sxs-lookup"><span data-stu-id="7ef17-148">Relationships</span></span>
|<span data-ttu-id="7ef17-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="7ef17-149">Relationship</span></span>|<span data-ttu-id="7ef17-150">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef17-150">Type</span></span>|<span data-ttu-id="7ef17-151">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef17-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef17-152">assignments</span><span class="sxs-lookup"><span data-stu-id="7ef17-152">assignments</span></span>|<span data-ttu-id="7ef17-153">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7ef17-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7ef17-154">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="7ef17-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="7ef17-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7ef17-155">deviceStatuses</span></span>|<span data-ttu-id="7ef17-156">Коллекция [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="7ef17-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7ef17-157">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="7ef17-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="7ef17-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7ef17-158">userStatuses</span></span>|<span data-ttu-id="7ef17-159">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7ef17-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7ef17-160">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="7ef17-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="7ef17-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7ef17-161">deviceStatusSummary</span></span>|[<span data-ttu-id="7ef17-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7ef17-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="7ef17-163">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="7ef17-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="7ef17-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7ef17-164">userStatusSummary</span></span>|[<span data-ttu-id="7ef17-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="7ef17-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="7ef17-166">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="7ef17-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ef17-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ef17-167">JSON Representation</span></span>
<span data-ttu-id="7ef17-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ef17-168">Here is a JSON representation of the resource.</span></span>
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




