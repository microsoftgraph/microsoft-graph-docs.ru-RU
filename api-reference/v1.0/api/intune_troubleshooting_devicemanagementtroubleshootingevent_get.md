# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="dadef-101">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="dadef-101">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="dadef-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dadef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dadef-103">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="dadef-103">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dadef-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dadef-104">Prerequisites</span></span>
<span data-ttu-id="dadef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dadef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dadef-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dadef-107">Permission type</span></span>|<span data-ttu-id="dadef-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dadef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dadef-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dadef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dadef-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dadef-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="dadef-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dadef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dadef-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dadef-112">Not supported.</span></span>|
|<span data-ttu-id="dadef-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dadef-113">Application</span></span>|<span data-ttu-id="dadef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dadef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dadef-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dadef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dadef-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dadef-116">Optional query parameters</span></span>
<span data-ttu-id="dadef-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dadef-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dadef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dadef-118">Request headers</span></span>
|<span data-ttu-id="dadef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dadef-119">Header</span></span>|<span data-ttu-id="dadef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dadef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dadef-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dadef-121">Authorization</span></span>|<span data-ttu-id="dadef-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="dadef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dadef-123">Принять</span><span class="sxs-lookup"><span data-stu-id="dadef-123">Accept</span></span>|<span data-ttu-id="dadef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dadef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dadef-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dadef-125">Request body</span></span>
<span data-ttu-id="dadef-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dadef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dadef-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dadef-127">Response</span></span>
<span data-ttu-id="dadef-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dadef-128">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dadef-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dadef-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dadef-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dadef-130">Request</span></span>
<span data-ttu-id="dadef-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dadef-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="dadef-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="dadef-132">Response</span></span>
<span data-ttu-id="dadef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dadef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```




