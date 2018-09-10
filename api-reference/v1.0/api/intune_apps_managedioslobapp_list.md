# <a name="list-managedioslobapps"></a><span data-ttu-id="8331e-101">Перечисление объектов managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="8331e-101">List managedIOSLobApps</span></span>

> <span data-ttu-id="8331e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8331e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8331e-103">Список свойств и связей объектов [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8331e-103">List properties and relationships of the [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8331e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8331e-104">Prerequisites</span></span>
<span data-ttu-id="8331e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8331e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8331e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8331e-107">Permission type</span></span>|<span data-ttu-id="8331e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8331e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8331e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8331e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8331e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8331e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8331e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8331e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8331e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8331e-112">Not supported.</span></span>|
|<span data-ttu-id="8331e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8331e-113">Application</span></span>|<span data-ttu-id="8331e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8331e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8331e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8331e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8331e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8331e-116">Request headers</span></span>
|<span data-ttu-id="8331e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8331e-117">Header</span></span>|<span data-ttu-id="8331e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8331e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8331e-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8331e-119">Authorization</span></span>|<span data-ttu-id="8331e-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8331e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8331e-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8331e-121">Accept</span></span>|<span data-ttu-id="8331e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8331e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8331e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8331e-123">Request body</span></span>
<span data-ttu-id="8331e-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8331e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8331e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8331e-125">Response</span></span>
<span data-ttu-id="8331e-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8331e-126">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8331e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8331e-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8331e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8331e-128">Request</span></span>
<span data-ttu-id="8331e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8331e-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="8331e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8331e-130">Response</span></span>
<span data-ttu-id="8331e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8331e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value"
    }
  ]
}
```








