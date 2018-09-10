# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="6f7f4-101">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6f7f4-101">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="6f7f4-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f7f4-103">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6f7f4-103">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f7f4-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7f4-104">Prerequisites</span></span>
<span data-ttu-id="6f7f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f7f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6f7f4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f7f4-107">Permission type</span></span>|<span data-ttu-id="6f7f4-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f7f4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f7f4-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f7f4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6f7f4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f7f4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f7f4-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f7f4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f7f4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-112">Not supported.</span></span>|
|<span data-ttu-id="6f7f4-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f7f4-113">Application</span></span>|<span data-ttu-id="6f7f4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f7f4-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f7f4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f7f4-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f7f4-116">Optional query parameters</span></span>
<span data-ttu-id="6f7f4-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6f7f4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f7f4-118">Request headers</span></span>
|<span data-ttu-id="6f7f4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f7f4-119">Header</span></span>|<span data-ttu-id="6f7f4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f7f4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f7f4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f7f4-121">Authorization</span></span>|<span data-ttu-id="6f7f4-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="6f7f4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f7f4-123">Принять</span><span class="sxs-lookup"><span data-stu-id="6f7f4-123">Accept</span></span>|<span data-ttu-id="6f7f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f7f4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f7f4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f7f4-125">Request body</span></span>
<span data-ttu-id="6f7f4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f7f4-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f7f4-127">Response</span></span>
<span data-ttu-id="6f7f4-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-128">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f7f4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6f7f4-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f7f4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f7f4-130">Request</span></span>
<span data-ttu-id="6f7f4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="6f7f4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f7f4-132">Response</span></span>
<span data-ttu-id="6f7f4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f7f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```








