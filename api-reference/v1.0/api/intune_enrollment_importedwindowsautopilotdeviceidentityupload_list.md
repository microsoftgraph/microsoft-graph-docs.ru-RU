# <a name="list-importedwindowsautopilotdeviceidentityuploads"></a><span data-ttu-id="8ce37-101">Список importedWindowsAutopilotDeviceIdentityUploads</span><span class="sxs-lookup"><span data-stu-id="8ce37-101">List importedWindowsAutopilotDeviceIdentityUploads</span></span>

> <span data-ttu-id="8ce37-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ce37-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ce37-103">Список свойств и связей объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="8ce37-103">List properties and relationships of the [managedDevice](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ce37-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ce37-104">Prerequisites</span></span>
<span data-ttu-id="8ce37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ce37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ce37-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce37-107">Permission type</span></span>|<span data-ttu-id="8ce37-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ce37-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ce37-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ce37-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ce37-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ce37-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8ce37-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ce37-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ce37-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce37-112">Not supported.</span></span>|
|<span data-ttu-id="8ce37-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ce37-113">Application</span></span>|<span data-ttu-id="8ce37-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce37-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ce37-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ce37-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="8ce37-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ce37-116">Request headers</span></span>
|<span data-ttu-id="8ce37-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ce37-117">Header</span></span>|<span data-ttu-id="8ce37-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8ce37-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ce37-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ce37-119">Authorization</span></span>|<span data-ttu-id="8ce37-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8ce37-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ce37-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8ce37-121">Accept</span></span>|<span data-ttu-id="8ce37-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="8ce37-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ce37-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ce37-123">Request body</span></span>
<span data-ttu-id="8ce37-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ce37-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ce37-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ce37-125">Response</span></span>
<span data-ttu-id="8ce37-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ce37-126">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ce37-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8ce37-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ce37-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ce37-128">Request</span></span>
<span data-ttu-id="8ce37-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ce37-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

### <a name="response"></a><span data-ttu-id="8ce37-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ce37-130">Response</span></span>
<span data-ttu-id="8ce37-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ce37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "8d639524-9524-8d63-2495-638d2495638d",
      "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
      "status": "pending"
    }
  ]
}
```








