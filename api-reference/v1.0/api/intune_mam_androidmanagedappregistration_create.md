# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="8980b-101">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8980b-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="8980b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8980b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8980b-103">Создание объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-103">Create a new [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8980b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8980b-104">Prerequisites</span></span>
<span data-ttu-id="8980b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8980b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8980b-107">Permission type</span></span>|<span data-ttu-id="8980b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8980b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8980b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8980b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8980b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8980b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8980b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8980b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8980b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8980b-112">Not supported.</span></span>|
|<span data-ttu-id="8980b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8980b-113">Application</span></span>|<span data-ttu-id="8980b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8980b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8980b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8980b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="8980b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8980b-116">Request headers</span></span>
|<span data-ttu-id="8980b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8980b-117">Header</span></span>|<span data-ttu-id="8980b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8980b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8980b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8980b-119">Authorization</span></span>|<span data-ttu-id="8980b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8980b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8980b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8980b-121">Accept</span></span>|<span data-ttu-id="8980b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8980b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8980b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8980b-123">Request body</span></span>
<span data-ttu-id="8980b-124">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8980b-124">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="8980b-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="8980b-125">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="8980b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8980b-126">Property</span></span>|<span data-ttu-id="8980b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8980b-127">Type</span></span>|<span data-ttu-id="8980b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8980b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8980b-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8980b-129">createdDateTime</span></span>|<span data-ttu-id="8980b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8980b-130">DateTimeOffset</span></span>|<span data-ttu-id="8980b-131">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8980b-132">lastSyncDateTime</span></span>|<span data-ttu-id="8980b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8980b-133">DateTimeOffset</span></span>|<span data-ttu-id="8980b-134">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="8980b-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="8980b-135">Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8980b-136">applicationVersion</span></span>|<span data-ttu-id="8980b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-137">String</span></span>|<span data-ttu-id="8980b-138">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8980b-139">managementSdkVersion</span></span>|<span data-ttu-id="8980b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-140">String</span></span>|<span data-ttu-id="8980b-141">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8980b-142">platformVersion</span></span>|<span data-ttu-id="8980b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-143">String</span></span>|<span data-ttu-id="8980b-144">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="8980b-145">deviceType</span></span>|<span data-ttu-id="8980b-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-146">String</span></span>|<span data-ttu-id="8980b-147">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8980b-148">deviceTag</span></span>|<span data-ttu-id="8980b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-149">String</span></span>|<span data-ttu-id="8980b-150">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="8980b-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8980b-151">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="8980b-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="8980b-152">Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="8980b-153">deviceName</span></span>|<span data-ttu-id="8980b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-154">String</span></span>|<span data-ttu-id="8980b-155">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8980b-156">flaggedReasons</span></span>|<span data-ttu-id="8980b-157">Коллекция перечисления[managedAppFlaggedReason enum](../resources/intune_mam_managedappflaggedreason.md)</span><span class="sxs-lookup"><span data-stu-id="8980b-157">[managedAppFlaggedReason enum](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="8980b-158">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="8980b-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8980b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="8980b-159">E.g.</span></span> <span data-ttu-id="8980b-160">Приложение запускается на административном устройстве. Унаследовано от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span> <span data-ttu-id="8980b-161">Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="8980b-161">The possible values are:</span></span>|
|<span data-ttu-id="8980b-162">userId</span><span class="sxs-lookup"><span data-stu-id="8980b-162">userId</span></span>|<span data-ttu-id="8980b-163">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-163">String</span></span>|<span data-ttu-id="8980b-164">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="8980b-164">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="8980b-165">Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-165">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-166">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8980b-166">appIdentifier</span></span>|[<span data-ttu-id="8980b-167">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8980b-167">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="8980b-168">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-168">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-169">id</span><span class="sxs-lookup"><span data-stu-id="8980b-169">id</span></span>|<span data-ttu-id="8980b-170">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-170">String</span></span>|<span data-ttu-id="8980b-171">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8980b-171">Key of the entity.</span></span> <span data-ttu-id="8980b-172">Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-172">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="8980b-173">version</span><span class="sxs-lookup"><span data-stu-id="8980b-173">version</span></span>|<span data-ttu-id="8980b-174">Строка</span><span class="sxs-lookup"><span data-stu-id="8980b-174">String</span></span>|<span data-ttu-id="8980b-175">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8980b-175">Version of the entity.</span></span> <span data-ttu-id="8980b-176">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="8980b-176">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8980b-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="8980b-177">Response</span></span>
<span data-ttu-id="8980b-178">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8980b-178">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8980b-179">Пример</span><span class="sxs-lookup"><span data-stu-id="8980b-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="8980b-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="8980b-180">Request</span></span>
<span data-ttu-id="8980b-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8980b-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8980b-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="8980b-182">Response</span></span>
<span data-ttu-id="8980b-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8980b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



