# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="ade92-101">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="ade92-101">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="ade92-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ade92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ade92-103">Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="ade92-103">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ade92-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ade92-104">Prerequisites</span></span>
<span data-ttu-id="ade92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ade92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ade92-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ade92-107">Permission type</span></span>|<span data-ttu-id="ade92-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ade92-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ade92-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ade92-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ade92-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ade92-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ade92-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ade92-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ade92-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade92-112">Not supported.</span></span>|
|<span data-ttu-id="ade92-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ade92-113">Application</span></span>|<span data-ttu-id="ade92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ade92-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ade92-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ade92-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ade92-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ade92-116">Optional query parameters</span></span>
<span data-ttu-id="ade92-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ade92-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ade92-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ade92-118">Request headers</span></span>
|<span data-ttu-id="ade92-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ade92-119">Header</span></span>|<span data-ttu-id="ade92-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ade92-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ade92-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ade92-121">Authorization</span></span>|<span data-ttu-id="ade92-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ade92-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ade92-123">Принять</span><span class="sxs-lookup"><span data-stu-id="ade92-123">Accept</span></span>|<span data-ttu-id="ade92-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ade92-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ade92-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ade92-125">Request body</span></span>
<span data-ttu-id="ade92-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ade92-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ade92-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ade92-127">Response</span></span>
<span data-ttu-id="ade92-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ade92-128">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ade92-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ade92-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ade92-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ade92-130">Request</span></span>
<span data-ttu-id="ade92-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ade92-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="ade92-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ade92-132">Response</span></span>
<span data-ttu-id="ade92-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ade92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
    "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
    "ruleName": "Rule Name value"
  }
}
```








