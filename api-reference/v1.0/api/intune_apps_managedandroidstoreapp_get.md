# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="f3565-101">Get managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f3565-101">Get managedAndroidStoreApp</span></span>

> <span data-ttu-id="f3565-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f3565-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3565-103">Чтение свойств и связей объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3565-103">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3565-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f3565-104">Prerequisites</span></span>
<span data-ttu-id="f3565-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3565-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3565-107">Permission type</span></span>|<span data-ttu-id="f3565-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3565-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3565-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3565-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f3565-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3565-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3565-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3565-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3565-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3565-112">Not supported.</span></span>|
|<span data-ttu-id="f3565-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3565-113">Application</span></span>|<span data-ttu-id="f3565-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3565-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3565-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3565-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3565-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3565-116">Optional query parameters</span></span>
<span data-ttu-id="f3565-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f3565-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f3565-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3565-118">Request headers</span></span>
|<span data-ttu-id="f3565-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3565-119">Header</span></span>|<span data-ttu-id="f3565-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f3565-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3565-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3565-121">Authorization</span></span>|<span data-ttu-id="f3565-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3565-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3565-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3565-123">Accept</span></span>|<span data-ttu-id="f3565-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3565-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3565-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3565-125">Request body</span></span>
<span data-ttu-id="f3565-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3565-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3565-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3565-127">Response</span></span>
<span data-ttu-id="f3565-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f3565-128">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3565-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f3565-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3565-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3565-130">Request</span></span>
<span data-ttu-id="f3565-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3565-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f3565-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3565-132">Response</span></span>
<span data-ttu-id="f3565-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f3565-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1275

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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



