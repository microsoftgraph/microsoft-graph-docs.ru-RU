# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="adbaa-101">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="adbaa-101">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="adbaa-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="adbaa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adbaa-103">Чтение свойств и связей объекта [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adbaa-103">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adbaa-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="adbaa-104">Prerequisites</span></span>
<span data-ttu-id="adbaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="adbaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="adbaa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adbaa-107">Permission type</span></span>|<span data-ttu-id="adbaa-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adbaa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adbaa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adbaa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="adbaa-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adbaa-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="adbaa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adbaa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adbaa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbaa-112">Not supported.</span></span>|
|<span data-ttu-id="adbaa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adbaa-113">Application</span></span>|<span data-ttu-id="adbaa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbaa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adbaa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adbaa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adbaa-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="adbaa-116">Optional query parameters</span></span>
<span data-ttu-id="adbaa-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="adbaa-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="adbaa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adbaa-118">Request headers</span></span>
|<span data-ttu-id="adbaa-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adbaa-119">Header</span></span>|<span data-ttu-id="adbaa-120">Значение</span><span class="sxs-lookup"><span data-stu-id="adbaa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adbaa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adbaa-121">Authorization</span></span>|<span data-ttu-id="adbaa-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adbaa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adbaa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="adbaa-123">Accept</span></span>|<span data-ttu-id="adbaa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="adbaa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adbaa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adbaa-125">Request body</span></span>
<span data-ttu-id="adbaa-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="adbaa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adbaa-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="adbaa-127">Response</span></span>
<span data-ttu-id="adbaa-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="adbaa-128">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbaa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="adbaa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="adbaa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbaa-130">Request</span></span>
<span data-ttu-id="adbaa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbaa-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="adbaa-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="adbaa-132">Response</span></span>
<span data-ttu-id="adbaa-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="adbaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
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
}
```



