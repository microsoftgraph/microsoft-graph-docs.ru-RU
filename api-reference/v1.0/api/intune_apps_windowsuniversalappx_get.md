# <a name="get-windowsuniversalappx"></a><span data-ttu-id="c1b8f-101">Get windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="c1b8f-101">Get windowsUniversalAppX</span></span>

> <span data-ttu-id="c1b8f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1b8f-103">Чтение свойств и связей объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-103">Read properties and relationships of the [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1b8f-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b8f-104">Prerequisites</span></span>
<span data-ttu-id="c1b8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1b8f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b8f-107">Permission type</span></span>|<span data-ttu-id="c1b8f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b8f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b8f-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1b8f-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1b8f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1b8f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b8f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-112">Not supported.</span></span>|
|<span data-ttu-id="c1b8f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1b8f-113">Application</span></span>|<span data-ttu-id="c1b8f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b8f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1b8f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1b8f-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1b8f-116">Optional query parameters</span></span>
<span data-ttu-id="c1b8f-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c1b8f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1b8f-118">Request headers</span></span>
|<span data-ttu-id="c1b8f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1b8f-119">Header</span></span>|<span data-ttu-id="c1b8f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c1b8f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b8f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1b8f-121">Authorization</span></span>|<span data-ttu-id="c1b8f-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c1b8f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b8f-123">Принять</span><span class="sxs-lookup"><span data-stu-id="c1b8f-123">Accept</span></span>|<span data-ttu-id="c1b8f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b8f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b8f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1b8f-125">Request body</span></span>
<span data-ttu-id="c1b8f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1b8f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1b8f-127">Response</span></span>
<span data-ttu-id="c1b8f-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-128">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b8f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c1b8f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1b8f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b8f-130">Request</span></span>
<span data-ttu-id="c1b8f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="c1b8f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1b8f-132">Response</span></span>
<span data-ttu-id="c1b8f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1b8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1450

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppX",
    "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "applicableDeviceTypes": "desktop",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true
    },
    "identityVersion": "Identity Version value"
  }
}
```








