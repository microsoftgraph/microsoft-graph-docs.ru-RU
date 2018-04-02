# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="aece0-101">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="aece0-101">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="aece0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aece0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aece0-103">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="aece0-103">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aece0-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="aece0-104">Prerequisites</span></span>
<span data-ttu-id="aece0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aece0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aece0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aece0-107">Permission type</span></span>|<span data-ttu-id="aece0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aece0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aece0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aece0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aece0-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="aece0-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="aece0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aece0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aece0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aece0-112">Not supported.</span></span>|
|<span data-ttu-id="aece0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aece0-113">Application</span></span>|<span data-ttu-id="aece0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aece0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aece0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aece0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="aece0-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aece0-116">Request headers</span></span>
|<span data-ttu-id="aece0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aece0-117">Header</span></span>|<span data-ttu-id="aece0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="aece0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aece0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aece0-119">Authorization</span></span>|<span data-ttu-id="aece0-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aece0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aece0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aece0-121">Accept</span></span>|<span data-ttu-id="aece0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aece0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aece0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aece0-123">Request body</span></span>
<span data-ttu-id="aece0-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aece0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aece0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="aece0-125">Response</span></span>
<span data-ttu-id="aece0-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aece0-126">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aece0-127">Пример</span><span class="sxs-lookup"><span data-stu-id="aece0-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="aece0-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="aece0-128">Request</span></span>
<span data-ttu-id="aece0-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aece0-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="aece0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="aece0-130">Response</span></span>
<span data-ttu-id="aece0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="aece0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "e4bede14-de14-e4be-14de-bee414debee4",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "available",
      "androidEnabled": true,
      "iosEnabled": true,
      "androidDeviceBlockedOnMissingPartnerData": true,
      "iosDeviceBlockedOnMissingPartnerData": true,
      "partnerUnsupportedOsVersionBlocked": true,
      "partnerUnresponsivenessThresholdInDays": 6
    }
  ]
}
```



