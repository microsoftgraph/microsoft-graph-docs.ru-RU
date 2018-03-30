# <a name="create-iosmanagedappregistration"></a><span data-ttu-id="9d8c6-101">Create iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9d8c6-101">Create iosManagedAppRegistration</span></span>

> <span data-ttu-id="9d8c6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d8c6-103">Создание объекта [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-103">Create a new [plannerBucket](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d8c6-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9d8c6-104">Prerequisites</span></span>
<span data-ttu-id="9d8c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d8c6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d8c6-107">Permission type</span></span>|<span data-ttu-id="9d8c6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d8c6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d8c6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d8c6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9d8c6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8c6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d8c6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d8c6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d8c6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-112">Not supported.</span></span>|
|<span data-ttu-id="9d8c6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d8c6-113">Application</span></span>|<span data-ttu-id="9d8c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d8c6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d8c6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="9d8c6-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d8c6-116">Request headers</span></span>
|<span data-ttu-id="9d8c6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d8c6-117">Header</span></span>|<span data-ttu-id="9d8c6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9d8c6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d8c6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d8c6-119">Authorization</span></span>|<span data-ttu-id="9d8c6-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d8c6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9d8c6-121">Accept</span></span>|<span data-ttu-id="9d8c6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9d8c6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d8c6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d8c6-123">Request body</span></span>
<span data-ttu-id="9d8c6-124">В тексте запроса добавьте представление объекта iosManagedAppRegistration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="9d8c6-125">В приведенной ниже таблице указаны свойства, необходимые для создания объекта iosManagedAppRegistration.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="9d8c6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d8c6-126">Property</span></span>|<span data-ttu-id="9d8c6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9d8c6-127">Type</span></span>|<span data-ttu-id="9d8c6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9d8c6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8c6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d8c6-129">createdDateTime</span></span>|<span data-ttu-id="9d8c6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d8c6-130">DateTimeOffset</span></span>|<span data-ttu-id="9d8c6-131">Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9d8c6-132">lastSyncDateTime</span></span>|<span data-ttu-id="9d8c6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d8c6-133">DateTimeOffset</span></span>|<span data-ttu-id="9d8c6-134">Дата и время последней синхронизации приложения со службой управления.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="9d8c6-135">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="9d8c6-136">applicationVersion</span></span>|<span data-ttu-id="9d8c6-137">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-137">String</span></span>|<span data-ttu-id="9d8c6-138">Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="9d8c6-139">managementSdkVersion</span></span>|<span data-ttu-id="9d8c6-140">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-140">String</span></span>|<span data-ttu-id="9d8c6-141">Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="9d8c6-142">platformVersion</span></span>|<span data-ttu-id="9d8c6-143">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-143">String</span></span>|<span data-ttu-id="9d8c6-144">Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="9d8c6-145">deviceType</span></span>|<span data-ttu-id="9d8c6-146">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-146">String</span></span>|<span data-ttu-id="9d8c6-147">Тип главного устройства. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9d8c6-148">deviceTag</span></span>|<span data-ttu-id="9d8c6-149">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-149">String</span></span>|<span data-ttu-id="9d8c6-150">Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="9d8c6-151">Мы не гарантируем, что приложения будут связаны во всех состояниях.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="9d8c6-152">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="9d8c6-153">deviceName</span></span>|<span data-ttu-id="9d8c6-154">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-154">String</span></span>|<span data-ttu-id="9d8c6-155">Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="9d8c6-156">flaggedReasons</span></span>|<span data-ttu-id="9d8c6-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9d8c6-157">String collection</span></span>|<span data-ttu-id="9d8c6-158">Причины, по которым помечается регистрация приложения (если они есть).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="9d8c6-159">Пример:</span><span class="sxs-lookup"><span data-stu-id="9d8c6-159">E.g.</span></span> <span data-ttu-id="9d8c6-160">приложение запускается на рутованном устройстве. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Возможные значения: `none`, `rootedDevice`.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="9d8c6-161">userId</span><span class="sxs-lookup"><span data-stu-id="9d8c6-161">userID</span></span>|<span data-ttu-id="9d8c6-162">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-162">String</span></span>|<span data-ttu-id="9d8c6-163">ИД пользователя, к которому относится эта регистрация приложения.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="9d8c6-164">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9d8c6-165">appIdentifier</span></span>|[<span data-ttu-id="9d8c6-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9d8c6-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="9d8c6-167">Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-168">id</span><span class="sxs-lookup"><span data-stu-id="9d8c6-168">id</span></span>|<span data-ttu-id="9d8c6-169">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-169">String</span></span>|<span data-ttu-id="9d8c6-170">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-170">Key of the setting.</span></span> <span data-ttu-id="9d8c6-171">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="9d8c6-172">version</span><span class="sxs-lookup"><span data-stu-id="9d8c6-172">version</span></span>|<span data-ttu-id="9d8c6-173">String</span><span class="sxs-lookup"><span data-stu-id="9d8c6-173">String</span></span>|<span data-ttu-id="9d8c6-174">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-174">Version of the entity.</span></span> <span data-ttu-id="9d8c6-175">Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9d8c6-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9d8c6-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d8c6-176">Response</span></span>
<span data-ttu-id="9d8c6-177">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-177">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d8c6-178">Пример</span><span class="sxs-lookup"><span data-stu-id="9d8c6-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d8c6-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d8c6-179">Request</span></span>
<span data-ttu-id="9d8c6-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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

### <a name="response"></a><span data-ttu-id="9d8c6-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d8c6-181">Response</span></span>
<span data-ttu-id="9d8c6-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9d8c6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



