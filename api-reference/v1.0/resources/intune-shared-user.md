---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7a6c87b5c073e00b660db807ff38c454c302d94
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253409"
---
# <a name="user-resource-type"></a><span data-ttu-id="bb202-103">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="bb202-103">user resource type</span></span>

> <span data-ttu-id="bb202-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb202-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb202-105">Представляет объект пользователя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb202-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="bb202-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bb202-106">Methods</span></span>
|<span data-ttu-id="bb202-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bb202-107">Method</span></span>|<span data-ttu-id="bb202-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb202-108">Return Type</span></span>|<span data-ttu-id="bb202-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb202-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb202-110">[Список](../api/intune-shared-user-list.md) объектов Users.</span><span class="sxs-lookup"><span data-stu-id="bb202-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="bb202-111">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="bb202-112">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="bb202-113">[Получение объекта User](../api/intune-shared-user-get.md) .</span><span class="sxs-lookup"><span data-stu-id="bb202-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="bb202-114">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="bb202-115">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="bb202-116">[Создание объекта User](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="bb202-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="bb202-117">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="bb202-118">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="bb202-119">[Удаление пользователя](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="bb202-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bb202-120">None</span></span>|<span data-ttu-id="bb202-121">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="bb202-122">[Обновление объекта пользователя](../api/intune-shared-user-update.md) .</span><span class="sxs-lookup"><span data-stu-id="bb202-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="bb202-123">user</span><span class="sxs-lookup"><span data-stu-id="bb202-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="bb202-124">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="bb202-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="bb202-125">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="bb202-125">**Device management**</span></span>|
|[<span data-ttu-id="bb202-126">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="bb202-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="bb202-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bb202-127">None</span></span>|<span data-ttu-id="bb202-128">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="bb202-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="bb202-129">**Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="bb202-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="bb202-130">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="bb202-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="bb202-131">Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="bb202-132">Получает состояние диагностической проверки определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb202-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="bb202-133">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="bb202-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="bb202-134">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bb202-135">Получает ограничения приложений для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb202-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="bb202-136">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="bb202-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="bb202-137">Нет</span><span class="sxs-lookup"><span data-stu-id="bb202-137">None</span></span>|<span data-ttu-id="bb202-138">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="bb202-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb202-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb202-139">Properties</span></span>
|<span data-ttu-id="bb202-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb202-140">Property</span></span>|<span data-ttu-id="bb202-141">Тип</span><span class="sxs-lookup"><span data-stu-id="bb202-141">Type</span></span>|<span data-ttu-id="bb202-142">Описание</span><span class="sxs-lookup"><span data-stu-id="bb202-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb202-143">id</span><span class="sxs-lookup"><span data-stu-id="bb202-143">id</span></span>|<span data-ttu-id="bb202-144">String</span><span class="sxs-lookup"><span data-stu-id="bb202-144">String</span></span>|<span data-ttu-id="bb202-145">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb202-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="bb202-146">**Подключение**</span><span class="sxs-lookup"><span data-stu-id="bb202-146">**Onboarding**</span></span>|
|<span data-ttu-id="bb202-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="bb202-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="bb202-148">Int32</span><span class="sxs-lookup"><span data-stu-id="bb202-148">Int32</span></span>|<span data-ttu-id="bb202-149">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="bb202-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="bb202-150">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="bb202-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="bb202-151">Связи</span><span class="sxs-lookup"><span data-stu-id="bb202-151">Relationships</span></span>
|<span data-ttu-id="bb202-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="bb202-152">Relationship</span></span>|<span data-ttu-id="bb202-153">Тип</span><span class="sxs-lookup"><span data-stu-id="bb202-153">Type</span></span>|<span data-ttu-id="bb202-154">Описание</span><span class="sxs-lookup"><span data-stu-id="bb202-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb202-155">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="bb202-155">**Device management**</span></span>|
|<span data-ttu-id="bb202-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="bb202-156">managedDevices</span></span>|<span data-ttu-id="bb202-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="bb202-158">Управляемые устройства, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="bb202-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="bb202-159">**Управление мобильным приложением (MAM)**</span><span class="sxs-lookup"><span data-stu-id="bb202-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="bb202-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="bb202-160">managedAppRegistrations</span></span>|<span data-ttu-id="bb202-161">Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="bb202-162">Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="bb202-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="bb202-163">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="bb202-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="bb202-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="bb202-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="bb202-165">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="bb202-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="bb202-166">Список событий устранения неполадок для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb202-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb202-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb202-167">JSON Representation</span></span>
<span data-ttu-id="bb202-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb202-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
