# <a name="manageddeviceenrollmenttopfailures-function"></a><span data-ttu-id="05336-101">Функция managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="05336-101">managedDeviceEnrollmentTopFailures function</span></span>

> <span data-ttu-id="05336-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05336-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05336-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05336-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05336-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="05336-104">Prerequisites</span></span>
<span data-ttu-id="05336-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05336-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05336-107">Permission type</span></span>|<span data-ttu-id="05336-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05336-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05336-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05336-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05336-110">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="05336-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="05336-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05336-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05336-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05336-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05336-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05336-113">Not supported.</span></span>|
|<span data-ttu-id="05336-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05336-114">Application</span></span>|<span data-ttu-id="05336-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05336-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05336-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05336-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentTopFailures
```

## <a name="request-headers"></a><span data-ttu-id="05336-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05336-117">Request headers</span></span>
|<span data-ttu-id="05336-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05336-118">Header</span></span>|<span data-ttu-id="05336-119">Значение</span><span class="sxs-lookup"><span data-stu-id="05336-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05336-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05336-120">Authorization</span></span>|<span data-ttu-id="05336-121">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="05336-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05336-122">Принять</span><span class="sxs-lookup"><span data-stu-id="05336-122">Accept</span></span>|<span data-ttu-id="05336-123">application/json</span><span class="sxs-lookup"><span data-stu-id="05336-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05336-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05336-124">Request body</span></span>
<span data-ttu-id="05336-125">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="05336-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="05336-126">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="05336-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="05336-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="05336-127">Property</span></span>|<span data-ttu-id="05336-128">Тип</span><span class="sxs-lookup"><span data-stu-id="05336-128">Type</span></span>|<span data-ttu-id="05336-129">Описание</span><span class="sxs-lookup"><span data-stu-id="05336-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05336-130">period</span><span class="sxs-lookup"><span data-stu-id="05336-130">period</span></span>|<span data-ttu-id="05336-131">String</span><span class="sxs-lookup"><span data-stu-id="05336-131">String</span></span>|<span data-ttu-id="05336-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05336-132">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05336-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="05336-133">Response</span></span>
<span data-ttu-id="05336-134">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune_shared_report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05336-134">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05336-135">Пример</span><span class="sxs-lookup"><span data-stu-id="05336-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="05336-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="05336-136">Request</span></span>
<span data-ttu-id="05336-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05336-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentTopFailures(period='parameterValue')
```

### <a name="response"></a><span data-ttu-id="05336-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="05336-138">Response</span></span>
<span data-ttu-id="05336-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05336-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




