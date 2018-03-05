# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="ae394-101">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ae394-101">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="ae394-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ae394-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae394-103">Чтение свойств и связей объекта [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ae394-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae394-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ae394-104">Prerequisites</span></span>
<span data-ttu-id="ae394-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae394-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae394-107">Permission type</span></span>|<span data-ttu-id="ae394-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae394-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae394-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae394-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ae394-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae394-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ae394-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae394-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae394-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae394-112">Not supported.</span></span>|
|<span data-ttu-id="ae394-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae394-113">Application</span></span>|<span data-ttu-id="ae394-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae394-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae394-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae394-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae394-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae394-116">Optional query parameters</span></span>
<span data-ttu-id="ae394-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae394-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae394-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae394-118">Request headers</span></span>
|<span data-ttu-id="ae394-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae394-119">Header</span></span>|<span data-ttu-id="ae394-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ae394-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae394-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae394-121">Authorization</span></span>|<span data-ttu-id="ae394-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae394-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae394-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ae394-123">Accept</span></span>|<span data-ttu-id="ae394-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ae394-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae394-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae394-125">Request body</span></span>
<span data-ttu-id="ae394-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae394-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae394-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae394-127">Response</span></span>
<span data-ttu-id="ae394-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae394-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae394-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ae394-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae394-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae394-130">Request</span></span>
<span data-ttu-id="ae394-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae394-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="ae394-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae394-132">Response</span></span>
<span data-ttu-id="ae394-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ae394-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```



