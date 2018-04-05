# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="abfcb-101">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="abfcb-101">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="abfcb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abfcb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abfcb-103">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="abfcb-103">Read properties and relationships of the [managedAppPolicy](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abfcb-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="abfcb-104">Prerequisites</span></span>
<span data-ttu-id="abfcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="abfcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="abfcb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abfcb-107">Permission type</span></span>|<span data-ttu-id="abfcb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abfcb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abfcb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abfcb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="abfcb-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="abfcb-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="abfcb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abfcb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abfcb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfcb-112">Not supported.</span></span>|
|<span data-ttu-id="abfcb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abfcb-113">Application</span></span>|<span data-ttu-id="abfcb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abfcb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abfcb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abfcb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abfcb-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abfcb-116">Optional query parameters</span></span>
<span data-ttu-id="abfcb-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="abfcb-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="abfcb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abfcb-118">Request headers</span></span>
|<span data-ttu-id="abfcb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abfcb-119">Header</span></span>|<span data-ttu-id="abfcb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="abfcb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abfcb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abfcb-121">Authorization</span></span>|<span data-ttu-id="abfcb-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abfcb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abfcb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="abfcb-123">Accept</span></span>|<span data-ttu-id="abfcb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="abfcb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abfcb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abfcb-125">Request body</span></span>
<span data-ttu-id="abfcb-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abfcb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abfcb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="abfcb-127">Response</span></span>
<span data-ttu-id="abfcb-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="abfcb-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abfcb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="abfcb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="abfcb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="abfcb-130">Request</span></span>
<span data-ttu-id="abfcb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abfcb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="abfcb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="abfcb-132">Response</span></span>
<span data-ttu-id="abfcb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="abfcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
    "serialNumber": "Serial Number value",
    "productKey": "Product Key value",
    "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
    "state": {
      "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
      "deviceImportStatus": "pending",
      "deviceRegistrationId": "Device Registration Id value",
      "deviceErrorCode": 15,
      "deviceErrorName": "Device Error Name value"
    }
  }
}
```



