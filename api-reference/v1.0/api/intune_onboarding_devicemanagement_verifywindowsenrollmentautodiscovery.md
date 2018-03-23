# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="b3cae-101">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="b3cae-101">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="b3cae-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3cae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3cae-103">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3cae-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3cae-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3cae-104">Prerequisites</span></span>
<span data-ttu-id="b3cae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b3cae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3cae-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3cae-107">Permission type</span></span>|<span data-ttu-id="b3cae-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3cae-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3cae-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3cae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b3cae-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3cae-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b3cae-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3cae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3cae-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3cae-112">Not supported.</span></span>|
|<span data-ttu-id="b3cae-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3cae-113">Application</span></span>|<span data-ttu-id="b3cae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3cae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3cae-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3cae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="b3cae-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3cae-116">Request headers</span></span>
|<span data-ttu-id="b3cae-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3cae-117">Header</span></span>|<span data-ttu-id="b3cae-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b3cae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3cae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3cae-119">Authorization</span></span>|<span data-ttu-id="b3cae-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3cae-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b3cae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b3cae-121">Accept</span></span>|<span data-ttu-id="b3cae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b3cae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3cae-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b3cae-123">Request body</span></span>
<span data-ttu-id="b3cae-124">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b3cae-124">In the request URL, provide the following required query parameters with values.</span></span>
<span data-ttu-id="b3cae-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="b3cae-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b3cae-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3cae-126">Property</span></span>|<span data-ttu-id="b3cae-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b3cae-127">Type</span></span>|<span data-ttu-id="b3cae-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b3cae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3cae-129">domainName</span><span class="sxs-lookup"><span data-stu-id="b3cae-129">domainName</span></span>|<span data-ttu-id="b3cae-130">String</span><span class="sxs-lookup"><span data-stu-id="b3cae-130">String</span></span>|<span data-ttu-id="b3cae-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b3cae-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b3cae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3cae-132">Response</span></span>
<span data-ttu-id="b3cae-133">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3cae-133">If successful, this method returns a `200 OK` response code and a sharedDriveItem resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3cae-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b3cae-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3cae-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3cae-135">Request</span></span>
<span data-ttu-id="b3cae-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3cae-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b3cae-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3cae-137">Response</span></span>
<span data-ttu-id="b3cae-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b3cae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



