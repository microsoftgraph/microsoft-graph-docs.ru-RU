# <a name="get-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="a6375-101">Получение importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="a6375-101">Get importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="a6375-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a6375-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6375-103">Чтение свойств и связей объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) .</span><span class="sxs-lookup"><span data-stu-id="a6375-103">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6375-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6375-104">Prerequisites</span></span>
<span data-ttu-id="a6375-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6375-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6375-107">Permission type</span></span>|<span data-ttu-id="a6375-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6375-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6375-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6375-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a6375-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6375-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6375-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6375-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6375-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6375-112">Not supported.</span></span>|
|<span data-ttu-id="a6375-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6375-113">Application</span></span>|<span data-ttu-id="a6375-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6375-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6375-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6375-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6375-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6375-116">Optional query parameters</span></span>
<span data-ttu-id="a6375-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6375-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a6375-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6375-118">Request headers</span></span>
|<span data-ttu-id="a6375-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6375-119">Header</span></span>|<span data-ttu-id="a6375-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a6375-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6375-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6375-121">Authorization</span></span>|<span data-ttu-id="a6375-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a6375-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6375-123">Принять</span><span class="sxs-lookup"><span data-stu-id="a6375-123">Accept</span></span>|<span data-ttu-id="a6375-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6375-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6375-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6375-125">Request body</span></span>
<span data-ttu-id="a6375-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6375-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6375-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6375-127">Response</span></span>
<span data-ttu-id="a6375-128">|||UNTRANSLATED_CONTENT_START|||If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="a6375-128">If successful, this method returns a `200 OK` response code and a [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6375-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a6375-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6375-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6375-130">Request</span></span>
<span data-ttu-id="a6375-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6375-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="a6375-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6375-132">Response</span></span>
<span data-ttu-id="a6375-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
    "id": "8d639524-9524-8d63-2495-638d2495638d",
    "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
    "status": "pending"
  }
}
```








