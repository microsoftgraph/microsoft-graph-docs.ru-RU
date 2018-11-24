# <a name="getauditcategories-function"></a><span data-ttu-id="bc639-101">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="bc639-101">getAuditCategories function</span></span>

> <span data-ttu-id="bc639-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc639-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc639-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bc639-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc639-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bc639-104">Prerequisites</span></span>
<span data-ttu-id="bc639-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc639-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc639-107">Permission type</span></span>|<span data-ttu-id="bc639-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc639-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc639-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc639-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bc639-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc639-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bc639-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc639-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc639-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc639-112">Not supported.</span></span>|
|<span data-ttu-id="bc639-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc639-113">Application</span></span>|<span data-ttu-id="bc639-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc639-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc639-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc639-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="bc639-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bc639-116">Request headers</span></span>
|<span data-ttu-id="bc639-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc639-117">Header</span></span>|<span data-ttu-id="bc639-118">Значение</span><span class="sxs-lookup"><span data-stu-id="bc639-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc639-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc639-119">Authorization</span></span>|<span data-ttu-id="bc639-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc639-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc639-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bc639-121">Accept</span></span>|<span data-ttu-id="bc639-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bc639-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc639-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc639-123">Request body</span></span>
<span data-ttu-id="bc639-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc639-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc639-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc639-125">Response</span></span>
<span data-ttu-id="bc639-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию String в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc639-126">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc639-127">Пример</span><span class="sxs-lookup"><span data-stu-id="bc639-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc639-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc639-128">Request</span></span>
<span data-ttu-id="bc639-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc639-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="bc639-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc639-130">Response</span></span>
<span data-ttu-id="bc639-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc639-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



