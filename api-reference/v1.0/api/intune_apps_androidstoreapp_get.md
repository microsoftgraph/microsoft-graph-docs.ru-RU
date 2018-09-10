# <a name="get-androidstoreapp"></a><span data-ttu-id="f9967-101">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f9967-101">Get androidStoreApp</span></span>

> <span data-ttu-id="f9967-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9967-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9967-103">Чтение свойств и связей объекта [androidStoreApp](../resources/intune_apps_androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9967-103">Read properties and relationships of the [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9967-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f9967-104">Prerequisites</span></span>
<span data-ttu-id="f9967-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9967-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9967-107">Permission type</span></span>|<span data-ttu-id="f9967-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9967-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9967-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9967-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f9967-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9967-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f9967-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9967-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9967-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9967-112">Not supported.</span></span>|
|<span data-ttu-id="f9967-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9967-113">Application</span></span>|<span data-ttu-id="f9967-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9967-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9967-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9967-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9967-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9967-116">Optional query parameters</span></span>
<span data-ttu-id="f9967-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9967-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f9967-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9967-118">Request headers</span></span>
|<span data-ttu-id="f9967-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9967-119">Header</span></span>|<span data-ttu-id="f9967-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f9967-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9967-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9967-121">Authorization</span></span>|<span data-ttu-id="f9967-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="f9967-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9967-123">Принять</span><span class="sxs-lookup"><span data-stu-id="f9967-123">Accept</span></span>|<span data-ttu-id="f9967-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f9967-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9967-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9967-125">Request body</span></span>
<span data-ttu-id="f9967-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9967-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9967-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9967-127">Response</span></span>
<span data-ttu-id="f9967-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidStoreApp](../resources/intune_apps_androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f9967-128">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune_apps_androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9967-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f9967-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9967-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9967-130">Request</span></span>
<span data-ttu-id="f9967-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9967-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f9967-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9967-132">Response</span></span>
<span data-ttu-id="f9967-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9967-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    }
  }
}
```








