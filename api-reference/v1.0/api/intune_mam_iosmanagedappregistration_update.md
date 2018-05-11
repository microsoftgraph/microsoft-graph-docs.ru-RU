# <a name="update-iosmanagedappregistration"></a><span data-ttu-id="be629-101">Обновление объекта iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="be629-101">Update iosManagedAppRegistration</span></span>

> <span data-ttu-id="be629-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be629-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be629-103">Обновление свойств объекта [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-103">Update the properties of a [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be629-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="be629-104">Prerequisites</span></span>
<span data-ttu-id="be629-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be629-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be629-107">Permission type</span></span>|<span data-ttu-id="be629-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be629-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be629-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be629-109">Delegated (work or school account)</span></span>|<span data-ttu-id="be629-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be629-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be629-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be629-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be629-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be629-112">Not supported.</span></span>|
|<span data-ttu-id="be629-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be629-113">Application</span></span>|<span data-ttu-id="be629-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be629-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be629-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be629-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="be629-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be629-116">Request headers</span></span>
|<span data-ttu-id="be629-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be629-117">Header</span></span>|<span data-ttu-id="be629-118">Значение</span><span class="sxs-lookup"><span data-stu-id="be629-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be629-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="be629-119">Authorization</span></span>|<span data-ttu-id="be629-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be629-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be629-121">Accept</span><span class="sxs-lookup"><span data-stu-id="be629-121">Accept</span></span>|<span data-ttu-id="be629-122">application/json</span><span class="sxs-lookup"><span data-stu-id="be629-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be629-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be629-123">Request body</span></span>
<span data-ttu-id="be629-124">В теле запроса добавьте представление объекта [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be629-124">In the request body, supply a JSON representation for the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>

<span data-ttu-id="be629-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-125">The following table shows the properties that are required when you create the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span></span>

|<span data-ttu-id="be629-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="be629-126">Property</span></span>|<span data-ttu-id="be629-127">Тип</span><span class="sxs-lookup"><span data-stu-id="be629-127">Type</span></span>|<span data-ttu-id="be629-128">Описание</span><span class="sxs-lookup"><span data-stu-id="be629-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be629-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be629-129">createdDateTime</span></span>|<span data-ttu-id="be629-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be629-130">DateTimeOffset</span></span>|<span data-ttu-id="be629-131">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="be629-132">lastSyncDateTime</span></span>|<span data-ttu-id="be629-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be629-133">DateTimeOffset</span></span>|<span data-ttu-id="be629-134">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="be629-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="be629-135">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="be629-136">applicationVersion</span></span>|<span data-ttu-id="be629-137">String</span><span class="sxs-lookup"><span data-stu-id="be629-137">String</span></span>|<span data-ttu-id="be629-138">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="be629-139">managementSdkVersion</span></span>|<span data-ttu-id="be629-140">String</span><span class="sxs-lookup"><span data-stu-id="be629-140">String</span></span>|<span data-ttu-id="be629-141">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="be629-142">platformVersion</span></span>|<span data-ttu-id="be629-143">String</span><span class="sxs-lookup"><span data-stu-id="be629-143">String</span></span>|<span data-ttu-id="be629-144">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="be629-145">deviceType</span></span>|<span data-ttu-id="be629-146">String</span><span class="sxs-lookup"><span data-stu-id="be629-146">String</span></span>|<span data-ttu-id="be629-147">Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="be629-148">deviceTag</span></span>|<span data-ttu-id="be629-149">String</span><span class="sxs-lookup"><span data-stu-id="be629-149">String</span></span>|<span data-ttu-id="be629-150">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="be629-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="be629-151">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="be629-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="be629-152">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="be629-153">deviceName</span></span>|<span data-ttu-id="be629-154">String</span><span class="sxs-lookup"><span data-stu-id="be629-154">String</span></span>|<span data-ttu-id="be629-155">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="be629-156">flaggedReasons</span></span>|<span data-ttu-id="be629-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="be629-157">String collection</span></span>|<span data-ttu-id="be629-158">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="be629-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="be629-159">Пример:</span><span class="sxs-lookup"><span data-stu-id="be629-159">E.g.</span></span> <span data-ttu-id="be629-160">приложение запускается на рутованном устройстве. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="be629-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="be629-161">userId</span><span class="sxs-lookup"><span data-stu-id="be629-161">userId</span></span>|<span data-ttu-id="be629-162">String</span><span class="sxs-lookup"><span data-stu-id="be629-162">String</span></span>|<span data-ttu-id="be629-163">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="be629-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="be629-164">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="be629-165">appIdentifier</span></span>|[<span data-ttu-id="be629-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="be629-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="be629-167">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-168">id</span><span class="sxs-lookup"><span data-stu-id="be629-168">id</span></span>|<span data-ttu-id="be629-169">String</span><span class="sxs-lookup"><span data-stu-id="be629-169">String</span></span>|<span data-ttu-id="be629-170">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be629-170">Key of the entity.</span></span> <span data-ttu-id="be629-171">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="be629-172">version</span><span class="sxs-lookup"><span data-stu-id="be629-172">version</span></span>|<span data-ttu-id="be629-173">String</span><span class="sxs-lookup"><span data-stu-id="be629-173">String</span></span>|<span data-ttu-id="be629-174">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="be629-174">Version of the entity.</span></span> <span data-ttu-id="be629-175">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="be629-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="be629-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="be629-176">Response</span></span>
<span data-ttu-id="be629-177">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be629-177">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be629-178">Пример</span><span class="sxs-lookup"><span data-stu-id="be629-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="be629-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="be629-179">Request</span></span>
<span data-ttu-id="be629-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be629-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 571

{
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
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="be629-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="be629-181">Response</span></span>
<span data-ttu-id="be629-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be629-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "id": "47632c19-2c19-4763-192c-6347192c6347",
  "version": "Version value"
}
```



