---
title: Тип ресурса restrictedAppsViolation
description: Нарушение профиля конфигурации ограниченных приложений каждого устройства на одного пользователя
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14979303c37cf189379a71b8cabc38f31e6b16b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923154"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="4427e-103">Тип ресурса restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="4427e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4427e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4427e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4427e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4427e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4427e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4427e-107">Нарушение профиля конфигурации ограниченных приложений каждого устройства на одного пользователя</span><span class="sxs-lookup"><span data-stu-id="4427e-107">Violation of restricted apps configuration profile per device per user</span></span>
## <a name="methods"></a><span data-ttu-id="4427e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4427e-108">Methods</span></span>
|<span data-ttu-id="4427e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4427e-109">Method</span></span>|<span data-ttu-id="4427e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4427e-110">Return Type</span></span>|<span data-ttu-id="4427e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4427e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4427e-112">Список restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="4427e-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="4427e-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4427e-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="4427e-114">Свойства списка и связей объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="4427e-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="4427e-115">Получение restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="4427e-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="4427e-117">Чтение свойства и связи объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="4427e-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="4427e-118">Создание restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="4427e-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="4427e-120">Создание нового объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="4427e-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="4427e-121">Удаление restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="4427e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4427e-122">None</span></span>|<span data-ttu-id="4427e-123">Удаляет [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="4427e-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="4427e-124">Обновление restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="4427e-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="4427e-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="4427e-126">Обновление свойства объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="4427e-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4427e-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="4427e-127">Properties</span></span>
|<span data-ttu-id="4427e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4427e-128">Property</span></span>|<span data-ttu-id="4427e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4427e-129">Type</span></span>|<span data-ttu-id="4427e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4427e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4427e-131">id</span><span class="sxs-lookup"><span data-stu-id="4427e-131">id</span></span>|<span data-ttu-id="4427e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4427e-132">String</span></span>|<span data-ttu-id="4427e-133">Уникальный идентификатор для объекта.</span><span class="sxs-lookup"><span data-stu-id="4427e-133">Unique identifier for the object.</span></span> <span data-ttu-id="4427e-134">Состоит из accountId, deviceId, policyId и идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="4427e-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="4427e-135">userId</span><span class="sxs-lookup"><span data-stu-id="4427e-135">userId</span></span>|<span data-ttu-id="4427e-136">String</span><span class="sxs-lookup"><span data-stu-id="4427e-136">String</span></span>|<span data-ttu-id="4427e-137">Уникальный идентификатор пользователя, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="4427e-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="4427e-138">userName</span><span class="sxs-lookup"><span data-stu-id="4427e-138">userName</span></span>|<span data-ttu-id="4427e-139">String</span><span class="sxs-lookup"><span data-stu-id="4427e-139">String</span></span>|<span data-ttu-id="4427e-140">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="4427e-140">User name</span></span>|
|<span data-ttu-id="4427e-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4427e-141">managedDeviceId</span></span>|<span data-ttu-id="4427e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4427e-142">String</span></span>|<span data-ttu-id="4427e-143">Уникальный идентификатор управляемого устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="4427e-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="4427e-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="4427e-144">deviceName</span></span>|<span data-ttu-id="4427e-145">String</span><span class="sxs-lookup"><span data-stu-id="4427e-145">String</span></span>|<span data-ttu-id="4427e-146">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="4427e-146">Device name</span></span>|
|<span data-ttu-id="4427e-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4427e-147">deviceConfigurationId</span></span>|<span data-ttu-id="4427e-148">Строка</span><span class="sxs-lookup"><span data-stu-id="4427e-148">String</span></span>|<span data-ttu-id="4427e-149">Конфигурация профиля уникальный идентификатор устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="4427e-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="4427e-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="4427e-150">deviceConfigurationName</span></span>|<span data-ttu-id="4427e-151">Строка</span><span class="sxs-lookup"><span data-stu-id="4427e-151">String</span></span>|<span data-ttu-id="4427e-152">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="4427e-152">Device configuration profile name</span></span>|
|<span data-ttu-id="4427e-153">platformType</span><span class="sxs-lookup"><span data-stu-id="4427e-153">platformType</span></span>|[<span data-ttu-id="4427e-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="4427e-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="4427e-155">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="4427e-155">Platform type.</span></span> <span data-ttu-id="4427e-156">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="4427e-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="4427e-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="4427e-157">restrictedAppsState</span></span>|[<span data-ttu-id="4427e-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="4427e-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="4427e-159">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="4427e-159">Restricted apps state.</span></span> <span data-ttu-id="4427e-160">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="4427e-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="4427e-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="4427e-161">restrictedApps</span></span>|<span data-ttu-id="4427e-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4427e-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="4427e-163">Список нарушенных ограниченных приложений</span><span class="sxs-lookup"><span data-stu-id="4427e-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="4427e-164">Связи</span><span class="sxs-lookup"><span data-stu-id="4427e-164">Relationships</span></span>
<span data-ttu-id="4427e-165">Нет</span><span class="sxs-lookup"><span data-stu-id="4427e-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4427e-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4427e-166">JSON Representation</span></span>
<span data-ttu-id="4427e-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4427e-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```





