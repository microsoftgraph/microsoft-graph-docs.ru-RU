# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="eaf02-101">Функция verifyWindowsEnrollmentAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="eaf02-101">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="eaf02-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eaf02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaf02-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eaf02-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eaf02-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eaf02-104">Prerequisites</span></span>
<span data-ttu-id="eaf02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eaf02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eaf02-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf02-107">Permission type</span></span>|<span data-ttu-id="eaf02-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf02-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf02-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf02-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eaf02-110">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="eaf02-110">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="eaf02-111">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf02-111">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf02-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf02-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf02-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf02-113">Not supported.</span></span>|
|<span data-ttu-id="eaf02-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf02-114">Application</span></span>|<span data-ttu-id="eaf02-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf02-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf02-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf02-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="eaf02-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaf02-117">Request headers</span></span>
|<span data-ttu-id="eaf02-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaf02-118">Header</span></span>|<span data-ttu-id="eaf02-119">Значение</span><span class="sxs-lookup"><span data-stu-id="eaf02-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf02-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaf02-120">Authorization</span></span>|<span data-ttu-id="eaf02-121">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eaf02-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf02-122">Accept</span><span class="sxs-lookup"><span data-stu-id="eaf02-122">Accept</span></span>|<span data-ttu-id="eaf02-123">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf02-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf02-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaf02-124">Request body</span></span>
<span data-ttu-id="eaf02-125">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="eaf02-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="eaf02-126">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="eaf02-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="eaf02-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf02-127">Property</span></span>|<span data-ttu-id="eaf02-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf02-128">Type</span></span>|<span data-ttu-id="eaf02-129">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf02-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf02-130">domainName</span><span class="sxs-lookup"><span data-stu-id="eaf02-130">domainName</span></span>|<span data-ttu-id="eaf02-131">String</span><span class="sxs-lookup"><span data-stu-id="eaf02-131">String</span></span>|<span data-ttu-id="eaf02-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eaf02-132">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="eaf02-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf02-133">Response</span></span>
<span data-ttu-id="eaf02-134">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eaf02-134">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf02-135">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf02-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="eaf02-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf02-136">Request</span></span>
<span data-ttu-id="eaf02-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaf02-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="eaf02-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaf02-138">Response</span></span>
<span data-ttu-id="eaf02-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="eaf02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



