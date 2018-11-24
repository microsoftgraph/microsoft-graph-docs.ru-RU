# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="4f176-101">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f176-101">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="4f176-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f176-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f176-103">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f176-103">Update the properties of a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f176-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="4f176-104">Prerequisites</span></span>
<span data-ttu-id="4f176-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f176-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f176-107">Permission type</span></span>|<span data-ttu-id="4f176-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f176-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f176-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f176-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4f176-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f176-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f176-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f176-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f176-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f176-112">Not supported.</span></span>|
|<span data-ttu-id="4f176-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f176-113">Application</span></span>|<span data-ttu-id="4f176-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f176-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f176-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f176-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f176-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f176-116">Request headers</span></span>
|<span data-ttu-id="4f176-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f176-117">Header</span></span>|<span data-ttu-id="4f176-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4f176-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f176-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f176-119">Authorization</span></span>|<span data-ttu-id="4f176-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f176-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f176-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4f176-121">Accept</span></span>|<span data-ttu-id="4f176-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4f176-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f176-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f176-123">Request body</span></span>
<span data-ttu-id="4f176-124">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f176-124">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="4f176-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f176-125">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="4f176-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f176-126">Property</span></span>|<span data-ttu-id="4f176-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4f176-127">Type</span></span>|<span data-ttu-id="4f176-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4f176-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f176-129">id</span><span class="sxs-lookup"><span data-stu-id="4f176-129">id</span></span>|<span data-ttu-id="4f176-130">String</span><span class="sxs-lookup"><span data-stu-id="4f176-130">String</span></span>|<span data-ttu-id="4f176-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f176-131">Key of the entity.</span></span> <span data-ttu-id="4f176-132">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4f176-133">targetedMobileApps</span></span>|<span data-ttu-id="4f176-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f176-134">String collection</span></span>|<span data-ttu-id="4f176-135">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="4f176-135">the associated app.</span></span> <span data-ttu-id="4f176-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f176-137">createdDateTime</span></span>|<span data-ttu-id="4f176-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f176-138">DateTimeOffset</span></span>|<span data-ttu-id="4f176-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4f176-139">DateTime the object was created.</span></span> <span data-ttu-id="4f176-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-141">описание</span><span class="sxs-lookup"><span data-stu-id="4f176-141">description</span></span>|<span data-ttu-id="4f176-142">String</span><span class="sxs-lookup"><span data-stu-id="4f176-142">String</span></span>|<span data-ttu-id="4f176-143">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f176-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f176-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f176-145">lastModifiedDateTime</span></span>|<span data-ttu-id="4f176-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f176-146">DateTimeOffset</span></span>|<span data-ttu-id="4f176-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f176-147">DateTime the object was last modified.</span></span> <span data-ttu-id="4f176-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-149">displayName</span><span class="sxs-lookup"><span data-stu-id="4f176-149">displayName</span></span>|<span data-ttu-id="4f176-150">String</span><span class="sxs-lookup"><span data-stu-id="4f176-150">String</span></span>|<span data-ttu-id="4f176-151">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f176-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f176-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-153">версия</span><span class="sxs-lookup"><span data-stu-id="4f176-153">version</span></span>|<span data-ttu-id="4f176-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4f176-154">Int32</span></span>|<span data-ttu-id="4f176-155">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f176-155">Version of the device configuration.</span></span> <span data-ttu-id="4f176-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="4f176-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="4f176-157">encodedSettingXml</span></span>|<span data-ttu-id="4f176-158">Двоичный</span><span class="sxs-lookup"><span data-stu-id="4f176-158">Binary</span></span>|<span data-ttu-id="4f176-159">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="4f176-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="4f176-160">параметры</span><span class="sxs-lookup"><span data-stu-id="4f176-160">settings</span></span>|<span data-ttu-id="4f176-161">Сбор данных [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="4f176-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="4f176-162">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="4f176-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="4f176-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f176-163">Response</span></span>
<span data-ttu-id="4f176-164">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="4f176-164">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f176-165">Пример</span><span class="sxs-lookup"><span data-stu-id="4f176-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f176-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f176-166">Request</span></span>
<span data-ttu-id="4f176-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f176-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="4f176-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f176-168">Response</span></span>
<span data-ttu-id="4f176-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f176-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



