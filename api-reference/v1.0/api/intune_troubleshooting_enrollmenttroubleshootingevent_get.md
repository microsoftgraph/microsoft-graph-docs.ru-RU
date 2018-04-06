# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="7f109-101">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7f109-101">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="7f109-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f109-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f109-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f109-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f109-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f109-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f109-105">Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7f109-105">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f109-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7f109-106">Prerequisites</span></span>
<span data-ttu-id="7f109-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f109-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f109-109">Permission type</span></span>|<span data-ttu-id="7f109-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f109-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f109-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f109-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f109-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f109-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7f109-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f109-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f109-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f109-114">Not supported.</span></span>|
|<span data-ttu-id="7f109-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f109-115">Application</span></span>|<span data-ttu-id="7f109-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f109-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f109-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f109-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f109-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f109-118">Optional query parameters</span></span>
<span data-ttu-id="7f109-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f109-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f109-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f109-120">Request headers</span></span>
|<span data-ttu-id="7f109-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f109-121">Header</span></span>|<span data-ttu-id="7f109-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f109-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f109-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f109-123">Authorization</span></span>|<span data-ttu-id="7f109-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f109-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f109-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f109-125">Accept</span></span>|<span data-ttu-id="7f109-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f109-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f109-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f109-127">Request body</span></span>
<span data-ttu-id="7f109-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f109-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f109-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f109-129">Response</span></span>
<span data-ttu-id="7f109-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7f109-130">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f109-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7f109-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f109-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f109-132">Request</span></span>
<span data-ttu-id="7f109-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f109-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="7f109-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f109-134">Response</span></span>
<span data-ttu-id="7f109-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f109-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
    "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value",
    "managedDeviceIdentifier": "Managed Device Identifier value",
    "operatingSystem": "Operating System value",
    "osVersion": "Os Version value",
    "userId": "User Id value",
    "deviceId": "Device Id value",
    "enrollmentType": "userEnrollment",
    "failureCategory": "authentication",
    "failureReason": "Failure Reason value"
  }
}
```



