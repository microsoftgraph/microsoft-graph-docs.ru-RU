# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="04751-101">Функция managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="04751-101">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="04751-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04751-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04751-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04751-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04751-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="04751-104">Prerequisites</span></span>
<span data-ttu-id="04751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04751-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04751-107">Permission type</span></span>|<span data-ttu-id="04751-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04751-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04751-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04751-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04751-110">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="04751-110">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="04751-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04751-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="04751-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04751-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04751-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04751-113">Not supported.</span></span>|
|<span data-ttu-id="04751-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04751-114">Application</span></span>|<span data-ttu-id="04751-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04751-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04751-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04751-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="04751-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04751-117">Request headers</span></span>
|<span data-ttu-id="04751-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04751-118">Header</span></span>|<span data-ttu-id="04751-119">Значение</span><span class="sxs-lookup"><span data-stu-id="04751-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04751-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04751-120">Authorization</span></span>|<span data-ttu-id="04751-121">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="04751-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04751-122">Принять</span><span class="sxs-lookup"><span data-stu-id="04751-122">Accept</span></span>|<span data-ttu-id="04751-123">приложение/json</span><span class="sxs-lookup"><span data-stu-id="04751-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04751-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04751-124">Request body</span></span>
<span data-ttu-id="04751-125">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="04751-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="04751-126">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="04751-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="04751-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="04751-127">Property</span></span>|<span data-ttu-id="04751-128">Тип</span><span class="sxs-lookup"><span data-stu-id="04751-128">Type</span></span>|<span data-ttu-id="04751-129">Описание</span><span class="sxs-lookup"><span data-stu-id="04751-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04751-130">skip</span><span class="sxs-lookup"><span data-stu-id="04751-130">skip</span></span>|<span data-ttu-id="04751-131">Int32</span><span class="sxs-lookup"><span data-stu-id="04751-131">Int32</span></span>|<span data-ttu-id="04751-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04751-132">Not yet documented</span></span>|
|<span data-ttu-id="04751-133">top</span><span class="sxs-lookup"><span data-stu-id="04751-133">top</span></span>|<span data-ttu-id="04751-134">Int32</span><span class="sxs-lookup"><span data-stu-id="04751-134">Int32</span></span>|<span data-ttu-id="04751-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04751-135">Not yet documented</span></span>|
|<span data-ttu-id="04751-136">filter</span><span class="sxs-lookup"><span data-stu-id="04751-136">filter</span></span>|<span data-ttu-id="04751-137">Строка</span><span class="sxs-lookup"><span data-stu-id="04751-137">String</span></span>|<span data-ttu-id="04751-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04751-138">Not yet documented</span></span>|
|<span data-ttu-id="04751-139">skipToken</span><span class="sxs-lookup"><span data-stu-id="04751-139">skipToken</span></span>|<span data-ttu-id="04751-140">Строка</span><span class="sxs-lookup"><span data-stu-id="04751-140">String</span></span>|<span data-ttu-id="04751-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04751-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="04751-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="04751-142">Response</span></span>
<span data-ttu-id="04751-143">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune_shared_report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04751-143">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04751-144">Пример</span><span class="sxs-lookup"><span data-stu-id="04751-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="04751-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="04751-145">Request</span></span>
<span data-ttu-id="04751-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04751-146">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="04751-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="04751-147">Response</span></span>
<span data-ttu-id="04751-148">Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="04751-148">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="04751-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04751-149">All of the properties will be returned from an actual call.</span></span>

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




