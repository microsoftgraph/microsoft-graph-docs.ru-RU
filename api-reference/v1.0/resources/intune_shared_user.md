# <a name="user-resource-type"></a><span data-ttu-id="c8b9a-101">Тип ресурса user</span><span class="sxs-lookup"><span data-stu-id="c8b9a-101">user resource type</span></span>

> <span data-ttu-id="c8b9a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8b9a-103">Представляет объект пользователя Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-103">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="c8b9a-104">Методы</span><span class="sxs-lookup"><span data-stu-id="c8b9a-104">Methods</span></span>
|<span data-ttu-id="c8b9a-105">Метод</span><span class="sxs-lookup"><span data-stu-id="c8b9a-105">Method</span></span>|<span data-ttu-id="c8b9a-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c8b9a-106">Return Type</span></span>|<span data-ttu-id="c8b9a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c8b9a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8b9a-108">Объекты [List users](../api/intune_shared_user_list.md).</span><span class="sxs-lookup"><span data-stu-id="c8b9a-108">[List users](../api/intune_shared_user_list.md) objects.</span></span>|
|<span data-ttu-id="c8b9a-109">Объект[Get user](../api/intune_shared_user_get.md).</span><span class="sxs-lookup"><span data-stu-id="c8b9a-109">[Get user](../api/intune_shared_user_get.md) object.</span></span>|
|<span data-ttu-id="c8b9a-110">Объект [Create user](../api/intune_shared_user_create.md).</span><span class="sxs-lookup"><span data-stu-id="c8b9a-110">Create a new [user](../api/intune_shared_user_create.md) object.</span></span>|
|<span data-ttu-id="c8b9a-111">Объект [Delete user](../api/intune_shared_user_delete.md).</span><span class="sxs-lookup"><span data-stu-id="c8b9a-111">Delete user</span></span>|
|<span data-ttu-id="c8b9a-112">Объект [Update user](../api/intune_shared_user_update.md).</span><span class="sxs-lookup"><span data-stu-id="c8b9a-112">Update user object.</span></span>|
|<span data-ttu-id="c8b9a-113">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-113">**Device management**</span></span>|
|[<span data-ttu-id="c8b9a-114">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="c8b9a-114">removeAllDevicesFromManagement action</span></span>](../api/intune_shared_user_removealldevicesfrommanagement.md)|<span data-ttu-id="c8b9a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c8b9a-115">None</span></span>|<span data-ttu-id="c8b9a-116">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="c8b9a-116">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="c8b9a-117">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-117">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="c8b9a-118">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="c8b9a-118">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="c8b9a-119">Коллекция [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="c8b9a-120">Получает состояние диагностической проверки определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-120">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="c8b9a-121">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="c8b9a-121">getManagedAppPolicies function</span></span>](../api/intune_shared_user_getmanagedapppolicies.md)|<span data-ttu-id="c8b9a-122">Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="c8b9a-123">Получает ограничения приложений для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-123">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="c8b9a-124">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="c8b9a-124">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="c8b9a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c8b9a-125">None</span></span>|<span data-ttu-id="c8b9a-126">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-126">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8b9a-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8b9a-127">Properties</span></span>
|<span data-ttu-id="c8b9a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8b9a-128">Property</span></span>|<span data-ttu-id="c8b9a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c8b9a-129">Type</span></span>|<span data-ttu-id="c8b9a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c8b9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8b9a-131">id</span><span class="sxs-lookup"><span data-stu-id="c8b9a-131">id</span></span>|<span data-ttu-id="c8b9a-132">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-132">String</span></span>|<span data-ttu-id="c8b9a-133">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-133">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c8b9a-134">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-134">**On-boarding**</span></span>|
|<span data-ttu-id="c8b9a-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c8b9a-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c8b9a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c8b9a-136">Int32</span></span>|<span data-ttu-id="c8b9a-137">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c8b9a-138">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-138">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c8b9a-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c8b9a-139">Relationships</span></span>
|<span data-ttu-id="c8b9a-140">Связь</span><span class="sxs-lookup"><span data-stu-id="c8b9a-140">Relationship</span></span>|<span data-ttu-id="c8b9a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="c8b9a-141">Type</span></span>|<span data-ttu-id="c8b9a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="c8b9a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8b9a-143">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-143">**Device management**</span></span>|
|<span data-ttu-id="c8b9a-144">managedDevices</span><span class="sxs-lookup"><span data-stu-id="c8b9a-144">managedDevices</span></span>|<span data-ttu-id="c8b9a-145">Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-145">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="c8b9a-146">Управляемые устройства, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-146">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="c8b9a-147">**Мобильное приложение управления (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-147">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="c8b9a-148">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c8b9a-148">managedAppRegistrations</span></span>|<span data-ttu-id="c8b9a-149">Коллекция [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="c8b9a-150">Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-150">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="c8b9a-151">**Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c8b9a-151">**Troubleshooting**</span></span>|
|<span data-ttu-id="c8b9a-152">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c8b9a-152">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="c8b9a-153">Коллекция [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="c8b9a-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c8b9a-154">Список событий устранения неполадок для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-154">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8b9a-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8b9a-155">JSON Representation</span></span>
<span data-ttu-id="c8b9a-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8b9a-156">Here is a JSON representation of the resource.</span></span>
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
