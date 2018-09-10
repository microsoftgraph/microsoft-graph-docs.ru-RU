# <a name="get-ioscertificateprofile"></a><span data-ttu-id="78c21-101">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="78c21-101">Get iosCertificateProfile</span></span>

> <span data-ttu-id="78c21-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78c21-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c21-103">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune_deviceconfig_ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="78c21-103">Read properties and relationships of the [iosCertificateProfile](../resources/intune_deviceconfig_ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78c21-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="78c21-104">Prerequisites</span></span>
<span data-ttu-id="78c21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="78c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="78c21-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78c21-107">Permission type</span></span>|<span data-ttu-id="78c21-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78c21-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78c21-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78c21-109">Delegated (work or school account)</span></span>|<span data-ttu-id="78c21-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78c21-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="78c21-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78c21-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78c21-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c21-112">Not supported.</span></span>|
|<span data-ttu-id="78c21-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78c21-113">Application</span></span>|<span data-ttu-id="78c21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78c21-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78c21-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78c21-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78c21-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="78c21-116">Optional query parameters</span></span>
<span data-ttu-id="78c21-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="78c21-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78c21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78c21-118">Request headers</span></span>
|<span data-ttu-id="78c21-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78c21-119">Header</span></span>|<span data-ttu-id="78c21-120">Значение</span><span class="sxs-lookup"><span data-stu-id="78c21-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78c21-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78c21-121">Authorization</span></span>|<span data-ttu-id="78c21-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="78c21-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78c21-123">Принять</span><span class="sxs-lookup"><span data-stu-id="78c21-123">Accept</span></span>|<span data-ttu-id="78c21-124">application/json</span><span class="sxs-lookup"><span data-stu-id="78c21-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78c21-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78c21-125">Request body</span></span>
<span data-ttu-id="78c21-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78c21-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78c21-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="78c21-127">Response</span></span>
<span data-ttu-id="78c21-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune_deviceconfig_ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="78c21-128">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune_deviceconfig_ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78c21-129">Пример</span><span class="sxs-lookup"><span data-stu-id="78c21-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="78c21-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="78c21-130">Request</span></span>
<span data-ttu-id="78c21-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78c21-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="78c21-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="78c21-132">Response</span></span>
<span data-ttu-id="78c21-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="78c21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```








