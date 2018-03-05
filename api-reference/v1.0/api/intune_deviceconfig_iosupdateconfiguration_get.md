# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="0a25b-101">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="0a25b-101">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="0a25b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a25b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a25b-103">Чтение свойств и связей объекта [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a25b-103">Read properties and relationships of [plannerBucketTaskBoardTaskFormat](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a25b-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0a25b-104">Prerequisites</span></span>
<span data-ttu-id="0a25b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a25b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a25b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a25b-107">Permission type</span></span>|<span data-ttu-id="0a25b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a25b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a25b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a25b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0a25b-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a25b-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0a25b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a25b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a25b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a25b-112">Not supported.</span></span>|
|<span data-ttu-id="0a25b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a25b-113">Application</span></span>|<span data-ttu-id="0a25b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a25b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a25b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a25b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a25b-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a25b-116">Optional query parameters</span></span>
<span data-ttu-id="0a25b-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0a25b-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0a25b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a25b-118">Request headers</span></span>
|<span data-ttu-id="0a25b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a25b-119">Header</span></span>|<span data-ttu-id="0a25b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0a25b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a25b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a25b-121">Authorization</span></span>|<span data-ttu-id="0a25b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a25b-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a25b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0a25b-123">Accept</span></span>|<span data-ttu-id="0a25b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a25b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a25b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a25b-125">Request body</span></span>
<span data-ttu-id="0a25b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a25b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a25b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a25b-127">Response</span></span>
<span data-ttu-id="0a25b-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a25b-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a25b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0a25b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a25b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a25b-130">Request</span></span>
<span data-ttu-id="0a25b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a25b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="0a25b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a25b-132">Response</span></span>
<span data-ttu-id="0a25b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0a25b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```



