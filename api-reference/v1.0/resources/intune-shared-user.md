---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
ms.openlocfilehash: 5d1d8e18e120fb26cfd5cea1cd223a6c38ad0aa9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027050"
---
# <a name="user-resource-type"></a><span data-ttu-id="5f64d-103">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="5f64d-103">user resource type</span></span>

> <span data-ttu-id="5f64d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f64d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f64d-105">Представляет объект пользователя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f64d-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="5f64d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5f64d-106">Methods</span></span>
|<span data-ttu-id="5f64d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5f64d-107">Method</span></span>|<span data-ttu-id="5f64d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5f64d-108">Return Type</span></span>|<span data-ttu-id="5f64d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f64d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f64d-110">Объекты [список пользователей](../api/intune-shared-user-list.md) .</span><span class="sxs-lookup"><span data-stu-id="5f64d-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="5f64d-111">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="5f64d-112">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="5f64d-113">[Получение пользовательского](../api/intune-shared-user-get.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="5f64d-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="5f64d-114">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="5f64d-115">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="5f64d-116">Объект [Создать пользователя](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="5f64d-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="5f64d-117">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="5f64d-118">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="5f64d-119">[Удаление пользователя](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="5f64d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5f64d-120">None</span></span>|<span data-ttu-id="5f64d-121">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="5f64d-122">Объект [пользователя обновления](../api/intune-shared-user-update.md) .</span><span class="sxs-lookup"><span data-stu-id="5f64d-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="5f64d-123">user</span><span class="sxs-lookup"><span data-stu-id="5f64d-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="5f64d-124">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5f64d-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="5f64d-125">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5f64d-125">**Device management**</span></span>|
|[<span data-ttu-id="5f64d-126">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="5f64d-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="5f64d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5f64d-127">None</span></span>|<span data-ttu-id="5f64d-128">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="5f64d-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="5f64d-129">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5f64d-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="5f64d-130">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="5f64d-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="5f64d-131">Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="5f64d-132">Получает состояние диагностической проверки определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f64d-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="5f64d-133">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="5f64d-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="5f64d-134">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5f64d-135">Получает ограничения приложений для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f64d-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="5f64d-136">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="5f64d-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="5f64d-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5f64d-137">None</span></span>|<span data-ttu-id="5f64d-138">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="5f64d-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f64d-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f64d-139">Properties</span></span>
|<span data-ttu-id="5f64d-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f64d-140">Property</span></span>|<span data-ttu-id="5f64d-141">Тип</span><span class="sxs-lookup"><span data-stu-id="5f64d-141">Type</span></span>|<span data-ttu-id="5f64d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5f64d-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f64d-143">id</span><span class="sxs-lookup"><span data-stu-id="5f64d-143">id</span></span>|<span data-ttu-id="5f64d-144">String</span><span class="sxs-lookup"><span data-stu-id="5f64d-144">String</span></span>|<span data-ttu-id="5f64d-145">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f64d-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="5f64d-146">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="5f64d-146">**Onboarding**</span></span>|
|<span data-ttu-id="5f64d-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="5f64d-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="5f64d-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5f64d-148">Int32</span></span>|<span data-ttu-id="5f64d-149">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="5f64d-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="5f64d-150">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="5f64d-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5f64d-151">Связи</span><span class="sxs-lookup"><span data-stu-id="5f64d-151">Relationships</span></span>
|<span data-ttu-id="5f64d-152">Связь</span><span class="sxs-lookup"><span data-stu-id="5f64d-152">Relationship</span></span>|<span data-ttu-id="5f64d-153">Тип</span><span class="sxs-lookup"><span data-stu-id="5f64d-153">Type</span></span>|<span data-ttu-id="5f64d-154">Description</span><span class="sxs-lookup"><span data-stu-id="5f64d-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f64d-155">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="5f64d-155">**Device management**</span></span>|
|<span data-ttu-id="5f64d-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="5f64d-156">managedDevices</span></span>|<span data-ttu-id="5f64d-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="5f64d-158">Управляемые устройства, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="5f64d-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="5f64d-159">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="5f64d-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="5f64d-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="5f64d-160">managedAppRegistrations</span></span>|<span data-ttu-id="5f64d-161">Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="5f64d-162">Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="5f64d-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="5f64d-163">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="5f64d-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="5f64d-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="5f64d-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="5f64d-165">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="5f64d-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="5f64d-166">Список событий устранения неполадок для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f64d-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f64d-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f64d-167">JSON Representation</span></span>
<span data-ttu-id="5f64d-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f64d-168">Here is a JSON representation of the resource.</span></span>
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
