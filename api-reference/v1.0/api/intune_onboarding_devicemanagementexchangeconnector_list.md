# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="012fc-101">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="012fc-101">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="012fc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="012fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="012fc-103">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="012fc-103">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="012fc-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="012fc-104">Prerequisites</span></span>
<span data-ttu-id="012fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="012fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="012fc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="012fc-107">Permission type</span></span>|<span data-ttu-id="012fc-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="012fc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="012fc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="012fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="012fc-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="012fc-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="012fc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="012fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="012fc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="012fc-112">Not supported.</span></span>|
|<span data-ttu-id="012fc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="012fc-113">Application</span></span>|<span data-ttu-id="012fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="012fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="012fc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="012fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="012fc-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="012fc-116">Request headers</span></span>
|<span data-ttu-id="012fc-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="012fc-117">Header</span></span>|<span data-ttu-id="012fc-118">Значение</span><span class="sxs-lookup"><span data-stu-id="012fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="012fc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="012fc-119">Authorization</span></span>|<span data-ttu-id="012fc-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="012fc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="012fc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="012fc-121">Accept</span></span>|<span data-ttu-id="012fc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="012fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="012fc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="012fc-123">Request body</span></span>
<span data-ttu-id="012fc-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="012fc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="012fc-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="012fc-125">Response</span></span>
<span data-ttu-id="012fc-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="012fc-126">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="012fc-127">Пример</span><span class="sxs-lookup"><span data-stu-id="012fc-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="012fc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="012fc-128">Request</span></span>
<span data-ttu-id="012fc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="012fc-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="012fc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="012fc-130">Response</span></span>
<span data-ttu-id="012fc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="012fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "status": "connectionPending",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "hosted",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```



