# <a name="get-devicecategory"></a><span data-ttu-id="937a7-101">Получение deviceCategory</span><span class="sxs-lookup"><span data-stu-id="937a7-101">Get deviceCategory</span></span>

> <span data-ttu-id="937a7-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="937a7-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="937a7-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937a7-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="937a7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="937a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="937a7-105">Чтение свойств и связей объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="937a7-105">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="937a7-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="937a7-106">Prerequisites</span></span>
<span data-ttu-id="937a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="937a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="937a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937a7-109">Permission type</span></span>|<span data-ttu-id="937a7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="937a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="937a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="937a7-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="937a7-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="937a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="937a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937a7-114">Not supported.</span></span>|
|<span data-ttu-id="937a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="937a7-115">Application</span></span>|<span data-ttu-id="937a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="937a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="937a7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="937a7-118">Optional query parameters</span></span>
<span data-ttu-id="937a7-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="937a7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="937a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="937a7-120">Request headers</span></span>
|<span data-ttu-id="937a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="937a7-121">Header</span></span>|<span data-ttu-id="937a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="937a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="937a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="937a7-123">Authorization</span></span>|<span data-ttu-id="937a7-124">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="937a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="937a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="937a7-125">Accept</span></span>|<span data-ttu-id="937a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="937a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="937a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="937a7-127">Request body</span></span>
<span data-ttu-id="937a7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="937a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="937a7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="937a7-129">Response</span></span>
<span data-ttu-id="937a7-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="937a7-130">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937a7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="937a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="937a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="937a7-132">Request</span></span>
<span data-ttu-id="937a7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="937a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="937a7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="937a7-134">Response</span></span>
<span data-ttu-id="937a7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="937a7-135">Here is an example of the response.</span></span> <span data-ttu-id="937a7-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="937a7-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="937a7-137">Свойства, возвращенные фактическим вызовом, могут различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="937a7-137">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



