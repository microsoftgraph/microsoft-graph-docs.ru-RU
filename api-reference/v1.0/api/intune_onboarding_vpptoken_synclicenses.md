# <a name="synclicenses-action"></a><span data-ttu-id="c2bc6-101">Действие syncLicenses</span><span class="sxs-lookup"><span data-stu-id="c2bc6-101">syncLicenses action</span></span>

> <span data-ttu-id="c2bc6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2bc6-103">Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken</span><span class="sxs-lookup"><span data-stu-id="c2bc6-103">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2bc6-104">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="c2bc6-104">Prerequisites</span></span>
<span data-ttu-id="c2bc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c2bc6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2bc6-107">Permission type</span></span>|<span data-ttu-id="c2bc6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2bc6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2bc6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2bc6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c2bc6-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2bc6-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c2bc6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2bc6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2bc6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-112">Not supported.</span></span>|
|<span data-ttu-id="c2bc6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2bc6-113">Application</span></span>|<span data-ttu-id="c2bc6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2bc6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2bc6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="c2bc6-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2bc6-116">Request headers</span></span>
|<span data-ttu-id="c2bc6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2bc6-117">Header</span></span>|<span data-ttu-id="c2bc6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c2bc6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2bc6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2bc6-119">Authorization</span></span>|<span data-ttu-id="c2bc6-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2bc6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c2bc6-121">Accept</span></span>|<span data-ttu-id="c2bc6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c2bc6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2bc6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2bc6-123">Request body</span></span>
<span data-ttu-id="c2bc6-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2bc6-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2bc6-125">Response</span></span>
<span data-ttu-id="c2bc6-126">При успешном выполнении данное действие возвращает `200 OK`код отклика и [vppToken](../resources/intune_onboarding_vpptoken.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-126">If successful, this action returns a  response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2bc6-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c2bc6-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2bc6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2bc6-128">Request</span></span>
<span data-ttu-id="c2bc6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="c2bc6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2bc6-130">Response</span></span>
<span data-ttu-id="c2bc6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2bc6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
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
}
```



