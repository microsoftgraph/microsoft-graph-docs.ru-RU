# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="f8b4d-101">Список объектов enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f8b4d-101">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="f8b4d-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b4d-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b4d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b4d-105">Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="f8b4d-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8b4d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8b4d-106">Prerequisites</span></span>
<span data-ttu-id="f8b4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8b4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f8b4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8b4d-109">Permission type</span></span>|<span data-ttu-id="f8b4d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8b4d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8b4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8b4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8b4d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8b4d-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f8b4d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8b4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8b4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-114">Not supported.</span></span>|
|<span data-ttu-id="f8b4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8b4d-115">Application</span></span>|<span data-ttu-id="f8b4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8b4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8b4d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f8b4d-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f8b4d-118">Request headers</span></span>
|<span data-ttu-id="f8b4d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8b4d-119">Header</span></span>|<span data-ttu-id="f8b4d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f8b4d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8b4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b4d-121">Authorization</span></span>|<span data-ttu-id="f8b4d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8b4d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f8b4d-123">Accept</span></span>|<span data-ttu-id="f8b4d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b4d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8b4d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8b4d-125">Request body</span></span>
<span data-ttu-id="f8b4d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8b4d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8b4d-127">Response</span></span>
<span data-ttu-id="f8b4d-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b4d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f8b4d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8b4d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8b4d-130">Request</span></span>
<span data-ttu-id="f8b4d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="f8b4d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8b4d-132">Response</span></span>
<span data-ttu-id="f8b4d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8b4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
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
  ]
}
```



