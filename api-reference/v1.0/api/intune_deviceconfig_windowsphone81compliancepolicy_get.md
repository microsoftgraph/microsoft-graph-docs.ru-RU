# <a name="get-windowsphone81compliancepolicy"></a><span data-ttu-id="4a17c-101">Get windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4a17c-101">Get windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="4a17c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4a17c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a17c-103">Чтение свойств и связей объекта [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4a17c-103">Read properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a17c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4a17c-104">Prerequisites</span></span>
<span data-ttu-id="4a17c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a17c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a17c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a17c-107">Permission type</span></span>|<span data-ttu-id="4a17c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a17c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a17c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a17c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4a17c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a17c-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a17c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a17c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a17c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a17c-112">Not supported.</span></span>|
|<span data-ttu-id="4a17c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a17c-113">Application</span></span>|<span data-ttu-id="4a17c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a17c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a17c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a17c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a17c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a17c-116">Optional query parameters</span></span>
<span data-ttu-id="4a17c-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a17c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4a17c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a17c-118">Request headers</span></span>
|<span data-ttu-id="4a17c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a17c-119">Header</span></span>|<span data-ttu-id="4a17c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4a17c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a17c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a17c-121">Authorization</span></span>|<span data-ttu-id="4a17c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a17c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a17c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4a17c-123">Accept</span></span>|<span data-ttu-id="4a17c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a17c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a17c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a17c-125">Request body</span></span>
<span data-ttu-id="4a17c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a17c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a17c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a17c-127">Response</span></span>
<span data-ttu-id="4a17c-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a17c-128">If successful, this method returns a `200 OK` response code and [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a17c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4a17c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a17c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a17c-130">Request</span></span>
<span data-ttu-id="4a17c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a17c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="4a17c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a17c-132">Response</span></span>
<span data-ttu-id="4a17c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4a17c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
    "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```



