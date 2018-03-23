# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="48c98-101">Создание объекта androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="48c98-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="48c98-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48c98-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48c98-103">Создание объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-103">Create a new [plannerBucket](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48c98-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48c98-104">Prerequisites</span></span>
<span data-ttu-id="48c98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48c98-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48c98-107">Permission type</span></span>|<span data-ttu-id="48c98-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48c98-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48c98-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48c98-109">Delegated (work or school account)</span></span>|<span data-ttu-id="48c98-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48c98-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48c98-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48c98-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48c98-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48c98-112">Not supported.</span></span>|
|<span data-ttu-id="48c98-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48c98-113">Application</span></span>|<span data-ttu-id="48c98-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48c98-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48c98-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48c98-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="48c98-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48c98-116">Request headers</span></span>
|<span data-ttu-id="48c98-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48c98-117">Header</span></span>|<span data-ttu-id="48c98-118">Значение</span><span class="sxs-lookup"><span data-stu-id="48c98-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48c98-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="48c98-119">Authorization</span></span>|<span data-ttu-id="48c98-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48c98-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="48c98-121">Accept</span><span class="sxs-lookup"><span data-stu-id="48c98-121">Accept</span></span>|<span data-ttu-id="48c98-122">application/json</span><span class="sxs-lookup"><span data-stu-id="48c98-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48c98-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48c98-123">Request body</span></span>
<span data-ttu-id="48c98-124">В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48c98-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="48c98-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="48c98-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="48c98-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="48c98-126">Property</span></span>|<span data-ttu-id="48c98-127">Тип</span><span class="sxs-lookup"><span data-stu-id="48c98-127">Type</span></span>|<span data-ttu-id="48c98-128">Описание</span><span class="sxs-lookup"><span data-stu-id="48c98-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48c98-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48c98-129">createdDateTime</span></span>|<span data-ttu-id="48c98-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48c98-130">DateTimeOffset</span></span>|<span data-ttu-id="48c98-131">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="48c98-132">lastSyncDateTime</span></span>|<span data-ttu-id="48c98-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48c98-133">DateTimeOffset</span></span>|<span data-ttu-id="48c98-134">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="48c98-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="48c98-135">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="48c98-136">applicationVersion</span></span>|<span data-ttu-id="48c98-137">String</span><span class="sxs-lookup"><span data-stu-id="48c98-137">String</span></span>|<span data-ttu-id="48c98-138">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="48c98-139">managementSdkVersion</span></span>|<span data-ttu-id="48c98-140">String</span><span class="sxs-lookup"><span data-stu-id="48c98-140">String</span></span>|<span data-ttu-id="48c98-141">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="48c98-142">platformVersion</span></span>|<span data-ttu-id="48c98-143">String</span><span class="sxs-lookup"><span data-stu-id="48c98-143">String</span></span>|<span data-ttu-id="48c98-144">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="48c98-145">deviceType</span></span>|<span data-ttu-id="48c98-146">String</span><span class="sxs-lookup"><span data-stu-id="48c98-146">String</span></span>|<span data-ttu-id="48c98-147">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="48c98-148">deviceTag</span></span>|<span data-ttu-id="48c98-149">String</span><span class="sxs-lookup"><span data-stu-id="48c98-149">String</span></span>|<span data-ttu-id="48c98-150">Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="48c98-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="48c98-151">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="48c98-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="48c98-152">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="48c98-153">deviceName</span></span>|<span data-ttu-id="48c98-154">String</span><span class="sxs-lookup"><span data-stu-id="48c98-154">String</span></span>|<span data-ttu-id="48c98-155">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="48c98-156">flaggedReasons</span></span>|<span data-ttu-id="48c98-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="48c98-157">String collection</span></span>|<span data-ttu-id="48c98-158">Нуль или более причин, по которым помечается регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="48c98-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="48c98-159">(например,</span><span class="sxs-lookup"><span data-stu-id="48c98-159">E.g.</span></span> <span data-ttu-id="48c98-160">приложение запускается на рутованном устройстве). Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="48c98-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="48c98-161">userId</span><span class="sxs-lookup"><span data-stu-id="48c98-161">userID</span></span>|<span data-ttu-id="48c98-162">String</span><span class="sxs-lookup"><span data-stu-id="48c98-162">String</span></span>|<span data-ttu-id="48c98-163">Идентификатор пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="48c98-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="48c98-164">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="48c98-165">appIdentifier</span></span>|[<span data-ttu-id="48c98-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="48c98-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="48c98-167">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-168">id</span><span class="sxs-lookup"><span data-stu-id="48c98-168">id</span></span>|<span data-ttu-id="48c98-169">String</span><span class="sxs-lookup"><span data-stu-id="48c98-169">String</span></span>|<span data-ttu-id="48c98-170">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48c98-170">Key of the setting.</span></span> <span data-ttu-id="48c98-171">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="48c98-172">version</span><span class="sxs-lookup"><span data-stu-id="48c98-172">version</span></span>|<span data-ttu-id="48c98-173">String</span><span class="sxs-lookup"><span data-stu-id="48c98-173">String</span></span>|<span data-ttu-id="48c98-174">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="48c98-174">Version of the entity.</span></span> <span data-ttu-id="48c98-175">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="48c98-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="48c98-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="48c98-176">Response</span></span>
<span data-ttu-id="48c98-177">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48c98-177">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48c98-178">Пример</span><span class="sxs-lookup"><span data-stu-id="48c98-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="48c98-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="48c98-179">Request</span></span>
<span data-ttu-id="48c98-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48c98-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48c98-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="48c98-181">Response</span></span>
<span data-ttu-id="48c98-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48c98-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



