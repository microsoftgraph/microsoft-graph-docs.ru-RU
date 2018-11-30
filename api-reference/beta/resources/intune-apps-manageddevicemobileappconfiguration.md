---
title: Тип ресурса managedDeviceMobileAppConfiguration
description: Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.
ms.openlocfilehash: c829e720e8d998428e778e5b7bf20e5fe465dfd6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074702"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="15753-103">Тип ресурса managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="15753-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="15753-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15753-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15753-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15753-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15753-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15753-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15753-107">Абстрактный класс для настройки мобильного приложения для зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="15753-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="15753-108">Методы</span><span class="sxs-lookup"><span data-stu-id="15753-108">Methods</span></span>
|<span data-ttu-id="15753-109">Метод</span><span class="sxs-lookup"><span data-stu-id="15753-109">Method</span></span>|<span data-ttu-id="15753-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15753-110">Return Type</span></span>|<span data-ttu-id="15753-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15753-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15753-112">Список managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="15753-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="15753-113">Коллекция [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15753-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="15753-114">Перечисление свойств и связей объектов [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15753-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="15753-115">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="15753-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="15753-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="15753-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="15753-117">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15753-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="15753-118">Действие assign</span><span class="sxs-lookup"><span data-stu-id="15753-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="15753-119">Нет</span><span class="sxs-lookup"><span data-stu-id="15753-119">None</span></span>|<span data-ttu-id="15753-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15753-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="15753-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="15753-121">Properties</span></span>
|<span data-ttu-id="15753-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="15753-122">Property</span></span>|<span data-ttu-id="15753-123">Тип</span><span class="sxs-lookup"><span data-stu-id="15753-123">Type</span></span>|<span data-ttu-id="15753-124">Описание</span><span class="sxs-lookup"><span data-stu-id="15753-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15753-125">id</span><span class="sxs-lookup"><span data-stu-id="15753-125">id</span></span>|<span data-ttu-id="15753-126">String</span><span class="sxs-lookup"><span data-stu-id="15753-126">String</span></span>|<span data-ttu-id="15753-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15753-127">Key of the entity.</span></span>|
|<span data-ttu-id="15753-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="15753-128">targetedMobileApps</span></span>|<span data-ttu-id="15753-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15753-129">String collection</span></span>|<span data-ttu-id="15753-130">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="15753-130">the associated app.</span></span>|
|<span data-ttu-id="15753-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15753-131">roleScopeTagIds</span></span>|<span data-ttu-id="15753-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15753-132">String collection</span></span>|<span data-ttu-id="15753-133">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="15753-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="15753-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15753-134">createdDateTime</span></span>|<span data-ttu-id="15753-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15753-135">DateTimeOffset</span></span>|<span data-ttu-id="15753-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15753-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="15753-137">описание</span><span class="sxs-lookup"><span data-stu-id="15753-137">description</span></span>|<span data-ttu-id="15753-138">String</span><span class="sxs-lookup"><span data-stu-id="15753-138">String</span></span>|<span data-ttu-id="15753-139">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15753-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="15753-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15753-140">lastModifiedDateTime</span></span>|<span data-ttu-id="15753-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15753-141">DateTimeOffset</span></span>|<span data-ttu-id="15753-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15753-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="15753-143">displayName</span><span class="sxs-lookup"><span data-stu-id="15753-143">displayName</span></span>|<span data-ttu-id="15753-144">String</span><span class="sxs-lookup"><span data-stu-id="15753-144">String</span></span>|<span data-ttu-id="15753-145">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15753-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="15753-146">version</span><span class="sxs-lookup"><span data-stu-id="15753-146">version</span></span>|<span data-ttu-id="15753-147">Int32</span><span class="sxs-lookup"><span data-stu-id="15753-147">Int32</span></span>|<span data-ttu-id="15753-148">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15753-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15753-149">Связи</span><span class="sxs-lookup"><span data-stu-id="15753-149">Relationships</span></span>
|<span data-ttu-id="15753-150">Связь</span><span class="sxs-lookup"><span data-stu-id="15753-150">Relationship</span></span>|<span data-ttu-id="15753-151">Тип</span><span class="sxs-lookup"><span data-stu-id="15753-151">Type</span></span>|<span data-ttu-id="15753-152">Описание</span><span class="sxs-lookup"><span data-stu-id="15753-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15753-153">assignments</span><span class="sxs-lookup"><span data-stu-id="15753-153">assignments</span></span>|<span data-ttu-id="15753-154">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="15753-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="15753-155">Список заданий группы для настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="15753-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="15753-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="15753-156">deviceStatuses</span></span>|<span data-ttu-id="15753-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="15753-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="15753-158">Список ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="15753-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="15753-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="15753-159">userStatuses</span></span>|<span data-ttu-id="15753-160">Коллекция [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="15753-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="15753-161">Список объектов ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="15753-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="15753-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="15753-162">deviceStatusSummary</span></span>|[<span data-ttu-id="15753-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="15753-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="15753-164">Общие сведения о состоянии устройства, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="15753-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="15753-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="15753-165">userStatusSummary</span></span>|[<span data-ttu-id="15753-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="15753-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="15753-167">Общие сведения о состоянии пользователя, связанном с настройкой приложения.</span><span class="sxs-lookup"><span data-stu-id="15753-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15753-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15753-168">JSON Representation</span></span>
<span data-ttu-id="15753-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15753-169">Here is a JSON representation of the resource.</span></span>
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





