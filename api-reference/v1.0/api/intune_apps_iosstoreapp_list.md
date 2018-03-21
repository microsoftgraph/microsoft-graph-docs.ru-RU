# <a name="list-iosstoreapps"></a><span data-ttu-id="5a171-101">Перечисление объектов iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="5a171-101">List iosStoreApps</span></span>

> <span data-ttu-id="5a171-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a171-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a171-103">Список свойств и связей объектов [iosStoreApp](../resources/intune_apps_iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a171-103">List properties and relationships of the [iosStoreApp](../resources/intune_apps_iosstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a171-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5a171-104">Prerequisites</span></span>
<span data-ttu-id="5a171-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a171-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a171-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a171-107">Permission type</span></span>|<span data-ttu-id="5a171-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a171-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a171-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a171-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a171-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a171-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5a171-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a171-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a171-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a171-112">Not supported.</span></span>|
|<span data-ttu-id="5a171-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a171-113">Application</span></span>|<span data-ttu-id="5a171-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a171-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a171-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a171-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5a171-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a171-116">Request headers</span></span>
|<span data-ttu-id="5a171-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a171-117">Header</span></span>|<span data-ttu-id="5a171-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5a171-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a171-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a171-119">Authorization</span></span>|<span data-ttu-id="5a171-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a171-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5a171-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5a171-121">Accept</span></span>|<span data-ttu-id="5a171-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a171-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a171-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a171-123">Request body</span></span>
<span data-ttu-id="5a171-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a171-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a171-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a171-125">Response</span></span>
<span data-ttu-id="5a171-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosStoreApp](../resources/intune_apps_iosstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a171-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_apps_iosstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a171-127">Пример</span><span class="sxs-lookup"><span data-stu-id="5a171-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a171-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a171-128">Request</span></span>
<span data-ttu-id="5a171-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a171-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="5a171-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a171-130">Response</span></span>
<span data-ttu-id="5a171-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5a171-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1323

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosStoreApp",
      "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  ]
}
```



