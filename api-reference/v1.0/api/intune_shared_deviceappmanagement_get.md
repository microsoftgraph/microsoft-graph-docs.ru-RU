# <a name="get-deviceappmanagement"></a><span data-ttu-id="ceb18-101">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="ceb18-101">Get deviceAppManagement</span></span>

> <span data-ttu-id="ceb18-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ceb18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ceb18-103">Чтение свойств и связей объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ceb18-103">Read properties and relationships of the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb18-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb18-104">Prerequisites</span></span>

<span data-ttu-id="ceb18-105">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ceb18-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ceb18-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ceb18-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="ceb18-107">Обратите внимание на то, что соответствующим разрешением изменяется в зависимости от рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="ceb18-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="ceb18-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb18-108">Permission type</span></span>|<span data-ttu-id="ceb18-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceb18-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb18-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceb18-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb18-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ceb18-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="ceb18-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceb18-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb18-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb18-113">Not supported.</span></span>|
|<span data-ttu-id="ceb18-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceb18-114">Application</span></span>|<span data-ttu-id="ceb18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb18-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb18-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceb18-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ceb18-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ceb18-117">Optional query parameters</span></span>
<span data-ttu-id="ceb18-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ceb18-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ceb18-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceb18-119">Request headers</span></span>
|<span data-ttu-id="ceb18-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ceb18-120">Header</span></span>|<span data-ttu-id="ceb18-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ceb18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceb18-122">Authorization</span></span>|<span data-ttu-id="ceb18-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ceb18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb18-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ceb18-124">Accept</span></span>|<span data-ttu-id="ceb18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb18-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceb18-126">Request body</span></span>
<span data-ttu-id="ceb18-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ceb18-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceb18-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceb18-128">Response</span></span>
<span data-ttu-id="ceb18-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ceb18-129">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="ceb18-130">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="ceb18-130">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="ceb18-131">Пример ответа</span><span class="sxs-lookup"><span data-stu-id="ceb18-131">Example response</span></span>
<span data-ttu-id="ceb18-132">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ceb18-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ceb18-133">Будут возвращены все свойства из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="ceb18-133">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



