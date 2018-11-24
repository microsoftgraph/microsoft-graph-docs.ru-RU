# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="26c30-101">Get iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="26c30-101">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="26c30-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="26c30-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26c30-103">Чтение свойств и связей объекта [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="26c30-103">Read properties and relationships of the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26c30-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="26c30-104">Prerequisites</span></span>
<span data-ttu-id="26c30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26c30-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26c30-107">Permission type</span></span>|<span data-ttu-id="26c30-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26c30-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26c30-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26c30-109">Delegated (work or school account)</span></span>|<span data-ttu-id="26c30-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="26c30-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="26c30-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26c30-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26c30-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26c30-112">Not supported.</span></span>|
|<span data-ttu-id="26c30-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26c30-113">Application</span></span>|<span data-ttu-id="26c30-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26c30-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26c30-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26c30-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26c30-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26c30-116">Optional query parameters</span></span>
<span data-ttu-id="26c30-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="26c30-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="26c30-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26c30-118">Request headers</span></span>
|<span data-ttu-id="26c30-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26c30-119">Header</span></span>|<span data-ttu-id="26c30-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26c30-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26c30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c30-121">Authorization</span></span>|<span data-ttu-id="26c30-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26c30-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26c30-123">Accept</span><span class="sxs-lookup"><span data-stu-id="26c30-123">Accept</span></span>|<span data-ttu-id="26c30-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26c30-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26c30-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26c30-125">Request body</span></span>
<span data-ttu-id="26c30-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26c30-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26c30-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="26c30-127">Response</span></span>
<span data-ttu-id="26c30-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="26c30-128">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c30-129">Пример</span><span class="sxs-lookup"><span data-stu-id="26c30-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="26c30-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="26c30-130">Request</span></span>
<span data-ttu-id="26c30-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26c30-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="26c30-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="26c30-132">Response</span></span>
<span data-ttu-id="26c30-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26c30-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 978

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true
  }
}
```



