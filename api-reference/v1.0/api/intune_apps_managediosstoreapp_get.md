# <a name="get-managediosstoreapp"></a><span data-ttu-id="b4b15-101">Get managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="b4b15-101">Get managedIOSStoreApp</span></span>

> <span data-ttu-id="b4b15-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b4b15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4b15-103">Чтение свойств и связей объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4b15-103">Read properties and relationships of the [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4b15-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b15-104">Prerequisites</span></span>
<span data-ttu-id="b4b15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4b15-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b15-107">Permission type</span></span>|<span data-ttu-id="b4b15-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4b15-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b15-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4b15-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b15-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b15-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4b15-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4b15-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b15-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b15-112">Not supported.</span></span>|
|<span data-ttu-id="b4b15-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4b15-113">Application</span></span>|<span data-ttu-id="b4b15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b15-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b15-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4b15-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4b15-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4b15-116">Optional query parameters</span></span>
<span data-ttu-id="b4b15-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4b15-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b4b15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4b15-118">Request headers</span></span>
|<span data-ttu-id="b4b15-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4b15-119">Header</span></span>|<span data-ttu-id="b4b15-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b4b15-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b15-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4b15-121">Authorization</span></span>|<span data-ttu-id="b4b15-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b4b15-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b15-123">Принять</span><span class="sxs-lookup"><span data-stu-id="b4b15-123">Accept</span></span>|<span data-ttu-id="b4b15-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b15-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b15-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4b15-125">Request body</span></span>
<span data-ttu-id="b4b15-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4b15-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4b15-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4b15-127">Response</span></span>
<span data-ttu-id="b4b15-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b4b15-128">If successful, this method returns a `200 OK` response code and [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b15-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b4b15-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4b15-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4b15-130">Request</span></span>
<span data-ttu-id="b4b15-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4b15-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="b4b15-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4b15-132">Response</span></span>
<span data-ttu-id="b4b15-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4b15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSStoreApp",
    "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
    "bundleId": "Bundle Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
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
    }
  }
}
```








