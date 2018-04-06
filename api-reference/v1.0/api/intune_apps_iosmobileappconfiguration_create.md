# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="bdd23-101">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdd23-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="bdd23-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bdd23-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdd23-103">Создание нового объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdd23-103">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdd23-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="bdd23-104">Prerequisites</span></span>
<span data-ttu-id="bdd23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdd23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bdd23-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd23-107">Permission type</span></span>|<span data-ttu-id="bdd23-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdd23-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdd23-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdd23-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bdd23-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd23-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bdd23-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdd23-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdd23-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd23-112">Not supported.</span></span>|
|<span data-ttu-id="bdd23-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdd23-113">Application</span></span>|<span data-ttu-id="bdd23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd23-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdd23-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdd23-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bdd23-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bdd23-116">Request headers</span></span>
|<span data-ttu-id="bdd23-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdd23-117">Header</span></span>|<span data-ttu-id="bdd23-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bdd23-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdd23-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdd23-119">Authorization</span></span>|<span data-ttu-id="bdd23-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdd23-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdd23-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bdd23-121">Accept</span></span>|<span data-ttu-id="bdd23-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bdd23-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdd23-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdd23-123">Request body</span></span>
<span data-ttu-id="bdd23-124">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdd23-124">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="bdd23-125">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bdd23-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="bdd23-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdd23-126">Property</span></span>|<span data-ttu-id="bdd23-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bdd23-127">Type</span></span>|<span data-ttu-id="bdd23-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bdd23-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd23-129">id</span><span class="sxs-lookup"><span data-stu-id="bdd23-129">id</span></span>|<span data-ttu-id="bdd23-130">String</span><span class="sxs-lookup"><span data-stu-id="bdd23-130">String</span></span>|<span data-ttu-id="bdd23-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bdd23-131">Key of the entity.</span></span> <span data-ttu-id="bdd23-132">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="bdd23-133">targetedMobileApps</span></span>|<span data-ttu-id="bdd23-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bdd23-134">String collection</span></span>|<span data-ttu-id="bdd23-135">приложение-обработчик.</span><span class="sxs-lookup"><span data-stu-id="bdd23-135">the associated app.</span></span> <span data-ttu-id="bdd23-136">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd23-137">createdDateTime</span></span>|<span data-ttu-id="bdd23-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd23-138">DateTimeOffset</span></span>|<span data-ttu-id="bdd23-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bdd23-139">DateTime the object was created.</span></span> <span data-ttu-id="bdd23-140">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-141">описание</span><span class="sxs-lookup"><span data-stu-id="bdd23-141">description</span></span>|<span data-ttu-id="bdd23-142">String</span><span class="sxs-lookup"><span data-stu-id="bdd23-142">String</span></span>|<span data-ttu-id="bdd23-143">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdd23-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bdd23-144">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdd23-145">lastModifiedDateTime</span></span>|<span data-ttu-id="bdd23-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdd23-146">DateTimeOffset</span></span>|<span data-ttu-id="bdd23-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bdd23-147">DateTime the object was last modified.</span></span> <span data-ttu-id="bdd23-148">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-149">displayName</span><span class="sxs-lookup"><span data-stu-id="bdd23-149">displayName</span></span>|<span data-ttu-id="bdd23-150">String</span><span class="sxs-lookup"><span data-stu-id="bdd23-150">String</span></span>|<span data-ttu-id="bdd23-151">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdd23-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bdd23-152">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-153">версия</span><span class="sxs-lookup"><span data-stu-id="bdd23-153">version</span></span>|<span data-ttu-id="bdd23-154">Int32</span><span class="sxs-lookup"><span data-stu-id="bdd23-154">Int32</span></span>|<span data-ttu-id="bdd23-155">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bdd23-155">Version of the device configuration.</span></span> <span data-ttu-id="bdd23-156">Унаследовано от[managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="bdd23-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="bdd23-157">encodedSettingXml</span></span>|<span data-ttu-id="bdd23-158">Двоичный</span><span class="sxs-lookup"><span data-stu-id="bdd23-158">Binary</span></span>|<span data-ttu-id="bdd23-159">двоичная конфигурация Base64 приложение службы управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="bdd23-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="bdd23-160">параметры</span><span class="sxs-lookup"><span data-stu-id="bdd23-160">settings</span></span>|<span data-ttu-id="bdd23-161">Сбор данных [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="bdd23-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="bdd23-162">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="bdd23-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="bdd23-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdd23-163">Response</span></span>
<span data-ttu-id="bdd23-164">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="bdd23-164">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdd23-165">Пример</span><span class="sxs-lookup"><span data-stu-id="bdd23-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdd23-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdd23-166">Request</span></span>
<span data-ttu-id="bdd23-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd23-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 598

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="bdd23-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdd23-168">Response</span></span>
<span data-ttu-id="bdd23-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bdd23-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



