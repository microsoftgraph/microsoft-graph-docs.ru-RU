# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="65483-101">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="65483-101">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="65483-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65483-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65483-103">Создание нового объекта [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65483-103">Create a new [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65483-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="65483-104">Prerequisites</span></span>
<span data-ttu-id="65483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65483-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65483-107">Permission type</span></span>|<span data-ttu-id="65483-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65483-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65483-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65483-109">Delegated (work or school account)</span></span>|<span data-ttu-id="65483-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65483-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65483-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65483-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65483-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65483-112">Not supported.</span></span>|
|<span data-ttu-id="65483-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65483-113">Application</span></span>|<span data-ttu-id="65483-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65483-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65483-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65483-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65483-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65483-116">Request headers</span></span>
|<span data-ttu-id="65483-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65483-117">Header</span></span>|<span data-ttu-id="65483-118">Значение</span><span class="sxs-lookup"><span data-stu-id="65483-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65483-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65483-119">Authorization</span></span>|<span data-ttu-id="65483-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="65483-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65483-121">Принять</span><span class="sxs-lookup"><span data-stu-id="65483-121">Accept</span></span>|<span data-ttu-id="65483-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65483-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65483-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65483-123">Request body</span></span>
<span data-ttu-id="65483-124">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65483-124">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="65483-125">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="65483-125">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="65483-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="65483-126">Property</span></span>|<span data-ttu-id="65483-127">Тип</span><span class="sxs-lookup"><span data-stu-id="65483-127">Type</span></span>|<span data-ttu-id="65483-128">Описание</span><span class="sxs-lookup"><span data-stu-id="65483-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65483-129">id</span><span class="sxs-lookup"><span data-stu-id="65483-129">id</span></span>|<span data-ttu-id="65483-130">Строка</span><span class="sxs-lookup"><span data-stu-id="65483-130">String</span></span>|<span data-ttu-id="65483-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65483-131">Key of the entity.</span></span> <span data-ttu-id="65483-132">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-132">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-133">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="65483-133">targetedMobileApps</span></span>|<span data-ttu-id="65483-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65483-134">String collection</span></span>|<span data-ttu-id="65483-135">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="65483-135">the associated app.</span></span> <span data-ttu-id="65483-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65483-137">createdDateTime</span></span>|<span data-ttu-id="65483-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65483-138">DateTimeOffset</span></span>|<span data-ttu-id="65483-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="65483-139">DateTime the object was created.</span></span> <span data-ttu-id="65483-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-141">описание</span><span class="sxs-lookup"><span data-stu-id="65483-141">description</span></span>|<span data-ttu-id="65483-142">Строка</span><span class="sxs-lookup"><span data-stu-id="65483-142">String</span></span>|<span data-ttu-id="65483-143">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="65483-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65483-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65483-145">lastModifiedDateTime</span></span>|<span data-ttu-id="65483-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65483-146">DateTimeOffset</span></span>|<span data-ttu-id="65483-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="65483-147">DateTime the object was last modified.</span></span> <span data-ttu-id="65483-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-149">displayName</span><span class="sxs-lookup"><span data-stu-id="65483-149">displayName</span></span>|<span data-ttu-id="65483-150">Строка</span><span class="sxs-lookup"><span data-stu-id="65483-150">String</span></span>|<span data-ttu-id="65483-151">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65483-151">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65483-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-153">версия</span><span class="sxs-lookup"><span data-stu-id="65483-153">version</span></span>|<span data-ttu-id="65483-154">Int32</span><span class="sxs-lookup"><span data-stu-id="65483-154">Int32</span></span>|<span data-ttu-id="65483-155">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65483-155">Version of the device configuration.</span></span> <span data-ttu-id="65483-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="65483-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="65483-157">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="65483-157">encodedSettingXml</span></span>|<span data-ttu-id="65483-158">Двоичный</span><span class="sxs-lookup"><span data-stu-id="65483-158">Binary</span></span>|<span data-ttu-id="65483-159">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="65483-159">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="65483-160">параметры</span><span class="sxs-lookup"><span data-stu-id="65483-160">settings</span></span>|<span data-ttu-id="65483-161">коллекция [appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="65483-161">[appConfigurationSettingItem](../resources/intune_apps_appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="65483-162">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="65483-162">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="65483-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="65483-163">Response</span></span>
<span data-ttu-id="65483-164">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="65483-164">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65483-165">Пример</span><span class="sxs-lookup"><span data-stu-id="65483-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="65483-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="65483-166">Request</span></span>
<span data-ttu-id="65483-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65483-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65483-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="65483-168">Response</span></span>
<span data-ttu-id="65483-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65483-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








