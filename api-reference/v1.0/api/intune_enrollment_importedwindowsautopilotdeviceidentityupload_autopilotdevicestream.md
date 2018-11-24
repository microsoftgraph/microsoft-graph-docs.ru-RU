# <a name="autopilotdevicestream-function"></a><span data-ttu-id="89593-101">функция autopilotDeviceStream</span><span class="sxs-lookup"><span data-stu-id="89593-101">autopilotDeviceStream function</span></span>

> <span data-ttu-id="89593-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="89593-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89593-103">Создание запроса загрузки с потоком автопилот устройство в нем.</span><span class="sxs-lookup"><span data-stu-id="89593-103">Create a upload request with autopilot device stream in it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89593-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="89593-104">Prerequisites</span></span>
<span data-ttu-id="89593-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="89593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89593-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89593-107">Permission type</span></span>|<span data-ttu-id="89593-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89593-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89593-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89593-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89593-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89593-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="89593-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89593-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89593-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89593-112">Not supported.</span></span>|
|<span data-ttu-id="89593-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89593-113">Application</span></span>|<span data-ttu-id="89593-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89593-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89593-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89593-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="89593-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89593-116">Request headers</span></span>
|<span data-ttu-id="89593-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89593-117">Header</span></span>|<span data-ttu-id="89593-118">Значение</span><span class="sxs-lookup"><span data-stu-id="89593-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89593-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="89593-119">Authorization</span></span>|<span data-ttu-id="89593-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89593-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89593-121">Accept</span><span class="sxs-lookup"><span data-stu-id="89593-121">Accept</span></span>|<span data-ttu-id="89593-122">application/json</span><span class="sxs-lookup"><span data-stu-id="89593-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89593-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89593-123">Request body</span></span>
<span data-ttu-id="89593-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89593-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89593-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="89593-125">Response</span></span>
<span data-ttu-id="89593-126">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89593-126">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89593-127">Пример</span><span class="sxs-lookup"><span data-stu-id="89593-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="89593-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="89593-128">Request</span></span>
<span data-ttu-id="89593-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89593-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="89593-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="89593-130">Response</span></span>
<span data-ttu-id="89593-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="89593-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



