# <a name="getauditactivitytypes-function"></a><span data-ttu-id="19696-101">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="19696-101">getAuditActivityTypes function</span></span>

> <span data-ttu-id="19696-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19696-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19696-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19696-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19696-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="19696-104">Prerequisites</span></span>
<span data-ttu-id="19696-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19696-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19696-107">Permission type</span></span>|<span data-ttu-id="19696-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19696-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19696-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19696-109">Delegated (work or school account)</span></span>|<span data-ttu-id="19696-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="19696-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="19696-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19696-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19696-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19696-112">Not supported.</span></span>|
|<span data-ttu-id="19696-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19696-113">Application</span></span>|<span data-ttu-id="19696-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19696-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19696-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19696-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="19696-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19696-116">Request headers</span></span>
|<span data-ttu-id="19696-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19696-117">Header</span></span>|<span data-ttu-id="19696-118">Значение</span><span class="sxs-lookup"><span data-stu-id="19696-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19696-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19696-119">Authorization</span></span>|<span data-ttu-id="19696-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="19696-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19696-121">Принять</span><span class="sxs-lookup"><span data-stu-id="19696-121">Accept</span></span>|<span data-ttu-id="19696-122">application/json</span><span class="sxs-lookup"><span data-stu-id="19696-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19696-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19696-123">Request body</span></span>
<span data-ttu-id="19696-124">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="19696-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="19696-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="19696-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="19696-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="19696-126">Property</span></span>|<span data-ttu-id="19696-127">Тип</span><span class="sxs-lookup"><span data-stu-id="19696-127">Type</span></span>|<span data-ttu-id="19696-128">Описание</span><span class="sxs-lookup"><span data-stu-id="19696-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19696-129">category</span><span class="sxs-lookup"><span data-stu-id="19696-129">category</span></span>|<span data-ttu-id="19696-130">Строка</span><span class="sxs-lookup"><span data-stu-id="19696-130">String</span></span>|<span data-ttu-id="19696-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19696-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="19696-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="19696-132">Response</span></span>
<span data-ttu-id="19696-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19696-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19696-134">Пример</span><span class="sxs-lookup"><span data-stu-id="19696-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="19696-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="19696-135">Request</span></span>
<span data-ttu-id="19696-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19696-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="19696-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="19696-137">Response</span></span>
<span data-ttu-id="19696-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19696-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








