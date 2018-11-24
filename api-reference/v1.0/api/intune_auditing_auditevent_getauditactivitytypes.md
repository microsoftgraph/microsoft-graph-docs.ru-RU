# <a name="getauditactivitytypes-function"></a><span data-ttu-id="ea7e8-101">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="ea7e8-101">getAuditActivityTypes function</span></span>

> <span data-ttu-id="ea7e8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea7e8-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea7e8-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea7e8-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea7e8-104">Prerequisites</span></span>
<span data-ttu-id="ea7e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea7e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea7e8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea7e8-107">Permission type</span></span>|<span data-ttu-id="ea7e8-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea7e8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea7e8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea7e8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ea7e8-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea7e8-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ea7e8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea7e8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea7e8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-112">Not supported.</span></span>|
|<span data-ttu-id="ea7e8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea7e8-113">Application</span></span>|<span data-ttu-id="ea7e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea7e8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea7e8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="ea7e8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea7e8-116">Request headers</span></span>
|<span data-ttu-id="ea7e8-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea7e8-117">Header</span></span>|<span data-ttu-id="ea7e8-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ea7e8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea7e8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea7e8-119">Authorization</span></span>|<span data-ttu-id="ea7e8-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea7e8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ea7e8-121">Accept</span></span>|<span data-ttu-id="ea7e8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ea7e8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea7e8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea7e8-123">Request body</span></span>
<span data-ttu-id="ea7e8-124">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ea7e8-125">В таблице ниже приведены параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ea7e8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea7e8-126">Property</span></span>|<span data-ttu-id="ea7e8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ea7e8-127">Type</span></span>|<span data-ttu-id="ea7e8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ea7e8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7e8-129">category</span><span class="sxs-lookup"><span data-stu-id="ea7e8-129">category</span></span>|<span data-ttu-id="ea7e8-130">String</span><span class="sxs-lookup"><span data-stu-id="ea7e8-130">String</span></span>|<span data-ttu-id="ea7e8-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea7e8-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ea7e8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea7e8-132">Response</span></span>
<span data-ttu-id="ea7e8-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7e8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ea7e8-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea7e8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea7e8-135">Request</span></span>
<span data-ttu-id="ea7e8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ea7e8-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea7e8-137">Response</span></span>
<span data-ttu-id="ea7e8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea7e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



