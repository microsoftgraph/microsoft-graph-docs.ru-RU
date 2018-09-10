# <a name="getauditcategories-function"></a><span data-ttu-id="fe65f-101">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="fe65f-101">getAuditCategories function</span></span>

> <span data-ttu-id="fe65f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe65f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe65f-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fe65f-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe65f-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fe65f-104">Prerequisites</span></span>
<span data-ttu-id="fe65f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe65f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe65f-107">Permission type</span></span>|<span data-ttu-id="fe65f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe65f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe65f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe65f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fe65f-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe65f-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fe65f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe65f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe65f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe65f-112">Not supported.</span></span>|
|<span data-ttu-id="fe65f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe65f-113">Application</span></span>|<span data-ttu-id="fe65f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe65f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe65f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe65f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="fe65f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe65f-116">Request headers</span></span>
|<span data-ttu-id="fe65f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe65f-117">Header</span></span>|<span data-ttu-id="fe65f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fe65f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe65f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe65f-119">Authorization</span></span>|<span data-ttu-id="fe65f-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fe65f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe65f-121">Принять</span><span class="sxs-lookup"><span data-stu-id="fe65f-121">Accept</span></span>|<span data-ttu-id="fe65f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fe65f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe65f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe65f-123">Request body</span></span>
<span data-ttu-id="fe65f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe65f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe65f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe65f-125">Response</span></span>
<span data-ttu-id="fe65f-126">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe65f-126">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe65f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fe65f-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe65f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe65f-128">Request</span></span>
<span data-ttu-id="fe65f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe65f-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="fe65f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe65f-130">Response</span></span>
<span data-ttu-id="fe65f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe65f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```








