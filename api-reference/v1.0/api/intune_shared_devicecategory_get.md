# <a name="get-devicecategory"></a><span data-ttu-id="9bb7e-101">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9bb7e-101">Get deviceCategory</span></span>



> <span data-ttu-id="9bb7e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bb7e-103">Чтение свойств и связей объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9bb7e-103">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bb7e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9bb7e-104">Prerequisites</span></span>
<span data-ttu-id="9bb7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9bb7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9bb7e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bb7e-107">Permission type</span></span>|<span data-ttu-id="9bb7e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bb7e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bb7e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bb7e-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9bb7e-110">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="9bb7e-110">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9bb7e-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bb7e-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="9bb7e-112">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="9bb7e-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9bb7e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bb7e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9bb7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bb7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bb7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-115">Not supported.</span></span>|
|<span data-ttu-id="9bb7e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bb7e-116">Application</span></span>|<span data-ttu-id="9bb7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bb7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bb7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bb7e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9bb7e-119">Optional query parameters</span></span>
<span data-ttu-id="9bb7e-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bb7e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bb7e-121">Request headers</span></span>
|<span data-ttu-id="9bb7e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bb7e-122">Header</span></span>|<span data-ttu-id="9bb7e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9bb7e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bb7e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bb7e-124">Authorization</span></span>|<span data-ttu-id="9bb7e-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9bb7e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bb7e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9bb7e-126">Accept</span></span>|<span data-ttu-id="9bb7e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9bb7e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bb7e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bb7e-128">Request body</span></span>
<span data-ttu-id="9bb7e-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bb7e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bb7e-130">Response</span></span>
<span data-ttu-id="9bb7e-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-131">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bb7e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9bb7e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bb7e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bb7e-133">Request</span></span>
<span data-ttu-id="9bb7e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="9bb7e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bb7e-135">Response</span></span>
<span data-ttu-id="9bb7e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-136">Here is an example of the response.</span></span> <span data-ttu-id="9bb7e-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9bb7e-138">Свойства, возвращенные фактический вызов различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="9bb7e-138">Properties returned from an actual call vary according to context.</span></span>

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



