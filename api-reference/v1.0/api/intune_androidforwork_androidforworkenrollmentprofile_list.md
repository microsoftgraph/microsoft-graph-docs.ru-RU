# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="10ebb-101">Перечисление объектов androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="10ebb-101">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="10ebb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10ebb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10ebb-103">Список свойств и связей объектов [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="10ebb-103">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10ebb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10ebb-104">Prerequisites</span></span>
<span data-ttu-id="10ebb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10ebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10ebb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ebb-107">Permission type</span></span>|<span data-ttu-id="10ebb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ebb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10ebb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ebb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="10ebb-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="10ebb-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="10ebb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ebb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ebb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ebb-112">Not supported.</span></span>|
|<span data-ttu-id="10ebb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ebb-113">Application</span></span>|<span data-ttu-id="10ebb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ebb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10ebb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ebb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="10ebb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ebb-116">Request headers</span></span>
|<span data-ttu-id="10ebb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10ebb-117">Header</span></span>|<span data-ttu-id="10ebb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="10ebb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10ebb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ebb-119">Authorization</span></span>|<span data-ttu-id="10ebb-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ebb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10ebb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="10ebb-121">Accept</span></span>|<span data-ttu-id="10ebb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="10ebb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ebb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ebb-123">Request body</span></span>
<span data-ttu-id="10ebb-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10ebb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ebb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ebb-125">Response</span></span>
<span data-ttu-id="10ebb-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10ebb-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ebb-127">Пример</span><span class="sxs-lookup"><span data-stu-id="10ebb-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="10ebb-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ebb-128">Request</span></span>
<span data-ttu-id="10ebb-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ebb-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="10ebb-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="10ebb-130">Response</span></span>
<span data-ttu-id="10ebb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10ebb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 926

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "e6742553-2553-e674-5325-74e6532574e6",
      "name": "Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "totalEnrollmentCount": 4,
      "enrolledDeviceCount": 3,
      "qrCode": "Qr Code value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ]
}
```



