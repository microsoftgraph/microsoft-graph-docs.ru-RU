# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="2a6b4-101">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a6b4-101">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="2a6b4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a6b4-103">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a6b4-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a6b4-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="2a6b4-104">Prerequisites</span></span>
<span data-ttu-id="2a6b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a6b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a6b4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a6b4-107">Permission type</span></span>|<span data-ttu-id="2a6b4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a6b4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a6b4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a6b4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a6b4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a6b4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-112">Not supported.</span></span>|
|<span data-ttu-id="2a6b4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a6b4-113">Application</span></span>|<span data-ttu-id="2a6b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a6b4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a6b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a6b4-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a6b4-116">Request headers</span></span>
|<span data-ttu-id="2a6b4-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a6b4-117">Header</span></span>|<span data-ttu-id="2a6b4-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2a6b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a6b4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a6b4-119">Authorization</span></span>|<span data-ttu-id="2a6b4-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a6b4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2a6b4-121">Accept</span></span>|<span data-ttu-id="2a6b4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a6b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a6b4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a6b4-123">Request body</span></span>
<span data-ttu-id="2a6b4-124">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-124">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="2a6b4-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a6b4-125">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune_apps_iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="2a6b4-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a6b4-126">Property</span></span>|<span data-ttu-id="2a6b4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2a6b4-127">Type</span></span>|<span data-ttu-id="2a6b4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2a6b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a6b4-129">id</span><span class="sxs-lookup"><span data-stu-id="2a6b4-129">id</span></span>|<span data-ttu-id="2a6b4-130">String</span><span class="sxs-lookup"><span data-stu-id="2a6b4-130">String</span></span>|<span data-ttu-id="2a6b4-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-131">Key of the entity.</span></span> <span data-ttu-id="2a6b4-132">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2a6b4-133">targetedMobileApps</span></span>|<span data-ttu-id="2a6b4-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2a6b4-134">String collection</span></span>|<span data-ttu-id="2a6b4-135">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="2a6b4-135">the associated app.</span></span> <span data-ttu-id="2a6b4-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a6b4-137">createdDateTime</span></span>|<span data-ttu-id="2a6b4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a6b4-138">DateTimeOffset</span></span>|<span data-ttu-id="2a6b4-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-139">DateTime the object was created.</span></span> <span data-ttu-id="2a6b4-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-141">описание</span><span class="sxs-lookup"><span data-stu-id="2a6b4-141">description</span></span>|<span data-ttu-id="2a6b4-142">String</span><span class="sxs-lookup"><span data-stu-id="2a6b4-142">String</span></span>|<span data-ttu-id="2a6b4-143">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2a6b4-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a6b4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2a6b4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a6b4-146">DateTimeOffset</span></span>|<span data-ttu-id="2a6b4-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-147">DateTime the object was last modified.</span></span> <span data-ttu-id="2a6b4-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-149">displayName</span><span class="sxs-lookup"><span data-stu-id="2a6b4-149">displayName</span></span>|<span data-ttu-id="2a6b4-150">String</span><span class="sxs-lookup"><span data-stu-id="2a6b4-150">String</span></span>|<span data-ttu-id="2a6b4-151">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2a6b4-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-153">версия</span><span class="sxs-lookup"><span data-stu-id="2a6b4-153">version</span></span>|<span data-ttu-id="2a6b4-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6b4-154">Int32</span></span>|<span data-ttu-id="2a6b4-155">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-155">Version of the device configuration.</span></span> <span data-ttu-id="2a6b4-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2a6b4-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="2a6b4-157">encodedSettingXml</span></span>|<span data-ttu-id="2a6b4-158">Двоичный</span><span class="sxs-lookup"><span data-stu-id="2a6b4-158">Binary</span></span>|<span data-ttu-id="2a6b4-159">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="2a6b4-160">параметры</span><span class="sxs-lookup"><span data-stu-id="2a6b4-160">settings</span></span>|<span data-ttu-id="2a6b4-161">Сбор данных [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="2a6b4-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="2a6b4-162">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="2a6b4-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a6b4-163">Response</span></span>
<span data-ttu-id="2a6b4-164">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-164">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppProtection](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a6b4-165">Пример</span><span class="sxs-lookup"><span data-stu-id="2a6b4-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a6b4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a6b4-166">Request</span></span>
<span data-ttu-id="2a6b4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2a6b4-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a6b4-168">Response</span></span>
<span data-ttu-id="2a6b4-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2a6b4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```



