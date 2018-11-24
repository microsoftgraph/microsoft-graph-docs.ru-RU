# <a name="get-reportroot"></a><span data-ttu-id="e13c4-101">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="e13c4-101">Get reportRoot</span></span>

> <span data-ttu-id="e13c4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e13c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e13c4-103">Чтение свойств и связей объекта [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="e13c4-103">Read properties and relationships of the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e13c4-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e13c4-104">Prerequisites</span></span>
<span data-ttu-id="e13c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e13c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e13c4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e13c4-107">Permission type</span></span>|<span data-ttu-id="e13c4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e13c4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e13c4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e13c4-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e13c4-110">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="e13c4-110">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="e13c4-111">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13c4-111">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e13c4-112">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e13c4-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e13c4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13c4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e13c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e13c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e13c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13c4-115">Not supported.</span></span>|
|<span data-ttu-id="e13c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e13c4-116">Application</span></span>|<span data-ttu-id="e13c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e13c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e13c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e13c4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e13c4-119">Optional query parameters</span></span>
<span data-ttu-id="e13c4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e13c4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e13c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e13c4-121">Request headers</span></span>
|<span data-ttu-id="e13c4-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e13c4-122">Header</span></span>|<span data-ttu-id="e13c4-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e13c4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e13c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e13c4-124">Authorization</span></span>|<span data-ttu-id="e13c4-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e13c4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e13c4-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e13c4-126">Accept</span></span>|<span data-ttu-id="e13c4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e13c4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e13c4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e13c4-128">Request body</span></span>
<span data-ttu-id="e13c4-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e13c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13c4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e13c4-130">Response</span></span>
<span data-ttu-id="e13c4-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune_shared_reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e13c4-131">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e13c4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e13c4-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="e13c4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e13c4-133">Request</span></span>
<span data-ttu-id="e13c4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e13c4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="e13c4-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e13c4-135">Response</span></span>
<span data-ttu-id="e13c4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e13c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








