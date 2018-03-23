# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="445de-101">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="445de-101">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="445de-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="445de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="445de-103">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="445de-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="445de-104">Prerequisites</span></span>
<span data-ttu-id="445de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="445de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="445de-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="445de-107">Permission type</span></span>|<span data-ttu-id="445de-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="445de-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="445de-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="445de-109">Delegated (work or school account)</span></span>|<span data-ttu-id="445de-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="445de-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="445de-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="445de-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="445de-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="445de-112">Not supported.</span></span>|
|<span data-ttu-id="445de-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="445de-113">Application</span></span>|<span data-ttu-id="445de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="445de-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="445de-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="445de-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="445de-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="445de-116">Request headers</span></span>
|<span data-ttu-id="445de-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="445de-117">Header</span></span>|<span data-ttu-id="445de-118">Значение</span><span class="sxs-lookup"><span data-stu-id="445de-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="445de-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="445de-119">Authorization</span></span>|<span data-ttu-id="445de-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="445de-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="445de-121">Accept</span><span class="sxs-lookup"><span data-stu-id="445de-121">Accept</span></span>|<span data-ttu-id="445de-122">application/json</span><span class="sxs-lookup"><span data-stu-id="445de-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="445de-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="445de-123">Request body</span></span>
<span data-ttu-id="445de-124">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="445de-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="445de-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="445de-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="445de-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="445de-126">Property</span></span>|<span data-ttu-id="445de-127">Тип</span><span class="sxs-lookup"><span data-stu-id="445de-127">Type</span></span>|<span data-ttu-id="445de-128">Описание</span><span class="sxs-lookup"><span data-stu-id="445de-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="445de-129">id</span><span class="sxs-lookup"><span data-stu-id="445de-129">id</span></span>|<span data-ttu-id="445de-130">String</span><span class="sxs-lookup"><span data-stu-id="445de-130">String</span></span>|<span data-ttu-id="445de-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="445de-131">Key of the setting.</span></span> <span data-ttu-id="445de-132">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="445de-133">lastModifiedDateTime</span></span>|<span data-ttu-id="445de-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="445de-134">DateTimeOffset</span></span>|<span data-ttu-id="445de-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="445de-135">DateTime the object was last modified.</span></span> <span data-ttu-id="445de-136">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="445de-137">createdDateTime</span></span>|<span data-ttu-id="445de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="445de-138">DateTimeOffset</span></span>|<span data-ttu-id="445de-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="445de-139">DateTime the object was created.</span></span> <span data-ttu-id="445de-140">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-141">description</span><span class="sxs-lookup"><span data-stu-id="445de-141">description</span></span>|<span data-ttu-id="445de-142">String</span><span class="sxs-lookup"><span data-stu-id="445de-142">String</span></span>|<span data-ttu-id="445de-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="445de-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="445de-144">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-145">displayName</span><span class="sxs-lookup"><span data-stu-id="445de-145">displayName</span></span>|<span data-ttu-id="445de-146">String</span><span class="sxs-lookup"><span data-stu-id="445de-146">String</span></span>|<span data-ttu-id="445de-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="445de-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="445de-148">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-149">version</span><span class="sxs-lookup"><span data-stu-id="445de-149">version</span></span>|<span data-ttu-id="445de-150">Int32</span><span class="sxs-lookup"><span data-stu-id="445de-150">Int32</span></span>|<span data-ttu-id="445de-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="445de-151">Version of the device configuration.</span></span> <span data-ttu-id="445de-152">Наследуется от объекта [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="445de-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="445de-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="445de-153">assetTagTemplate</span></span>|<span data-ttu-id="445de-154">String</span><span class="sxs-lookup"><span data-stu-id="445de-154">String</span></span>|<span data-ttu-id="445de-155">Сведения, касающиеся тега ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="445de-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="445de-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="445de-156">lockScreenFootnote</span></span>|<span data-ttu-id="445de-157">String</span><span class="sxs-lookup"><span data-stu-id="445de-157">String</span></span>|<span data-ttu-id="445de-158">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="445de-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="445de-159">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="445de-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="445de-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="445de-160">homeScreenDockIcons</span></span>|<span data-ttu-id="445de-161">Коллекция [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="445de-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="445de-162">Список приложений и папок, которые должны отображаться на панели задач на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="445de-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="445de-163">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="445de-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="445de-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="445de-164">homeScreenPages</span></span>|<span data-ttu-id="445de-165">Коллекция [iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="445de-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="445de-166">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="445de-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="445de-167">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="445de-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="445de-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="445de-168">notificationSettings</span></span>|<span data-ttu-id="445de-169">Коллекция [iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="445de-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="445de-170">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="445de-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="445de-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="445de-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="445de-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="445de-172">Response</span></span>
<span data-ttu-id="445de-173">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="445de-173">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="445de-174">Пример</span><span class="sxs-lookup"><span data-stu-id="445de-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="445de-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="445de-175">Request</span></span>
<span data-ttu-id="445de-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="445de-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2052

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="445de-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="445de-177">Response</span></span>
<span data-ttu-id="445de-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="445de-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```



