---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 908abafa3ace358125636b2c38e4cb751536a617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967365"
---
# <a name="user-resource-type"></a><span data-ttu-id="aff9a-103">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="aff9a-103">user resource type</span></span>

> <span data-ttu-id="aff9a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aff9a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aff9a-105">Представляет объект пользователя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="aff9a-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="aff9a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aff9a-106">Methods</span></span>
|<span data-ttu-id="aff9a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aff9a-107">Method</span></span>|<span data-ttu-id="aff9a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aff9a-108">Return Type</span></span>|<span data-ttu-id="aff9a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aff9a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff9a-110">Объекты [список пользователей](../api/intune-shared-user-list.md) .</span><span class="sxs-lookup"><span data-stu-id="aff9a-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="aff9a-111">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="aff9a-112">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="aff9a-113">[Получение пользовательского](../api/intune-shared-user-get.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="aff9a-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="aff9a-114">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="aff9a-115">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="aff9a-116">Объект [Создать пользователя](../api/intune-shared-user-create.md) .</span><span class="sxs-lookup"><span data-stu-id="aff9a-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="aff9a-117">Коллекция объектов [user](../resources/intune-shared-user.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="aff9a-118">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="aff9a-119">[Удаление пользователя](../api/intune-shared-user-delete.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="aff9a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="aff9a-120">None</span></span>|<span data-ttu-id="aff9a-121">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="aff9a-122">Объект [пользователя обновления](../api/intune-shared-user-update.md) .</span><span class="sxs-lookup"><span data-stu-id="aff9a-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="aff9a-123">user</span><span class="sxs-lookup"><span data-stu-id="aff9a-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="aff9a-124">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="aff9a-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="aff9a-125">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="aff9a-125">**Device management**</span></span>|
|[<span data-ttu-id="aff9a-126">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="aff9a-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="aff9a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="aff9a-127">None</span></span>|<span data-ttu-id="aff9a-128">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="aff9a-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="aff9a-129">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="aff9a-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="aff9a-130">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="aff9a-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="aff9a-131">Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="aff9a-132">Получает состояние диагностической проверки определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff9a-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="aff9a-133">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="aff9a-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="aff9a-134">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="aff9a-135">Получает ограничения приложений для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff9a-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="aff9a-136">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="aff9a-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="aff9a-137">Нет</span><span class="sxs-lookup"><span data-stu-id="aff9a-137">None</span></span>|<span data-ttu-id="aff9a-138">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="aff9a-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="aff9a-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff9a-139">Properties</span></span>
|<span data-ttu-id="aff9a-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff9a-140">Property</span></span>|<span data-ttu-id="aff9a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="aff9a-141">Type</span></span>|<span data-ttu-id="aff9a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="aff9a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff9a-143">id</span><span class="sxs-lookup"><span data-stu-id="aff9a-143">id</span></span>|<span data-ttu-id="aff9a-144">String</span><span class="sxs-lookup"><span data-stu-id="aff9a-144">String</span></span>|<span data-ttu-id="aff9a-145">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff9a-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="aff9a-146">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="aff9a-146">**Onboarding**</span></span>|
|<span data-ttu-id="aff9a-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="aff9a-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="aff9a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="aff9a-148">Int32</span></span>|<span data-ttu-id="aff9a-149">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="aff9a-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="aff9a-150">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="aff9a-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="aff9a-151">Связи</span><span class="sxs-lookup"><span data-stu-id="aff9a-151">Relationships</span></span>
|<span data-ttu-id="aff9a-152">Связь</span><span class="sxs-lookup"><span data-stu-id="aff9a-152">Relationship</span></span>|<span data-ttu-id="aff9a-153">Тип</span><span class="sxs-lookup"><span data-stu-id="aff9a-153">Type</span></span>|<span data-ttu-id="aff9a-154">Описание</span><span class="sxs-lookup"><span data-stu-id="aff9a-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff9a-155">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="aff9a-155">**Device management**</span></span>|
|<span data-ttu-id="aff9a-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="aff9a-156">managedDevices</span></span>|<span data-ttu-id="aff9a-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="aff9a-158">Управляемые устройства, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="aff9a-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="aff9a-159">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="aff9a-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="aff9a-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="aff9a-160">managedAppRegistrations</span></span>|<span data-ttu-id="aff9a-161">Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="aff9a-162">Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="aff9a-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="aff9a-163">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="aff9a-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="aff9a-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="aff9a-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="aff9a-165">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="aff9a-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="aff9a-166">Список событий устранения неполадок для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff9a-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aff9a-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff9a-167">JSON Representation</span></span>
<span data-ttu-id="aff9a-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff9a-168">Here is a JSON representation of the resource.</span></span>
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
