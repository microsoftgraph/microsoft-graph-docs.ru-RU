# <a name="list-vpptokens"></a><span data-ttu-id="7b203-101">Список VPP токенов</span><span class="sxs-lookup"><span data-stu-id="7b203-101">List vppTokens</span></span>

> <span data-ttu-id="7b203-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b203-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b203-103">Список свойств и связей объектов [VPP токены](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="7b203-103">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune_onboarding_vpptoken.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b203-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="7b203-104">Prerequisites</span></span>
<span data-ttu-id="7b203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b203-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b203-107">Permission type</span></span>|<span data-ttu-id="7b203-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b203-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b203-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b203-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7b203-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b203-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7b203-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b203-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b203-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b203-112">Not supported.</span></span>|
|<span data-ttu-id="7b203-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b203-113">Application</span></span>|<span data-ttu-id="7b203-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b203-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b203-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b203-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="7b203-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b203-116">Request headers</span></span>
|<span data-ttu-id="7b203-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b203-117">Header</span></span>|<span data-ttu-id="7b203-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7b203-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b203-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b203-119">Authorization</span></span>|<span data-ttu-id="7b203-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b203-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b203-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7b203-121">Accept</span></span>|<span data-ttu-id="7b203-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7b203-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b203-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b203-123">Request body</span></span>
<span data-ttu-id="7b203-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b203-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b203-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b203-125">Response</span></span>
<span data-ttu-id="7b203-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [VPP Токенов ](../resources/intune_onboarding_vpptoken.md) в текстовом поле для отклика.</span><span class="sxs-lookup"><span data-stu-id="7b203-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_onboarding_vpptoken.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b203-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7b203-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b203-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b203-128">Request</span></span>
<span data-ttu-id="7b203-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b203-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
```

### <a name="response"></a><span data-ttu-id="7b203-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b203-130">Response</span></span>
<span data-ttu-id="7b203-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7b203-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "education",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "valid",
      "lastSyncStatus": "inProgress",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```



