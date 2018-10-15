# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="b2190-101">Создание importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="b2190-101">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="b2190-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2190-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2190-103">Создание нового объекта [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="b2190-103">Create a new [deviceConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2190-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2190-104">Prerequisites</span></span>
<span data-ttu-id="b2190-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2190-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2190-107">Permission type</span></span>|<span data-ttu-id="b2190-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2190-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2190-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2190-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b2190-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2190-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b2190-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2190-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2190-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2190-112">Not supported.</span></span>|
|<span data-ttu-id="b2190-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2190-113">Application</span></span>|<span data-ttu-id="b2190-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2190-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2190-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2190-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="b2190-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2190-116">Request headers</span></span>
|<span data-ttu-id="b2190-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2190-117">Header</span></span>|<span data-ttu-id="b2190-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b2190-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2190-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2190-119">Authorization</span></span>|<span data-ttu-id="b2190-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b2190-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2190-121">Принять</span><span class="sxs-lookup"><span data-stu-id="b2190-121">Accept</span></span>|<span data-ttu-id="b2190-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="b2190-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2190-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2190-123">Request body</span></span>
<span data-ttu-id="b2190-124">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentityUpload в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2190-124">In the request body, supply a JSON representation for the targetedManagedAppPolicyAssignment object.</span></span>

<span data-ttu-id="b2190-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта  importedWindowsAutopilotDeviceIdentityUpload.</span><span class="sxs-lookup"><span data-stu-id="b2190-125">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="b2190-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2190-126">Property</span></span>|<span data-ttu-id="b2190-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b2190-127">Type</span></span>|<span data-ttu-id="b2190-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b2190-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2190-129">id</span><span class="sxs-lookup"><span data-stu-id="b2190-129">id</span></span>|<span data-ttu-id="b2190-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b2190-130">String</span></span>|<span data-ttu-id="b2190-131">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b2190-131">The GUID for the object</span></span>|
|<span data-ttu-id="b2190-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="b2190-132">createdDateTimeUtc</span></span>|<span data-ttu-id="b2190-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2190-133">DateTimeOffset</span></span>|<span data-ttu-id="b2190-134">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b2190-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="b2190-135">status</span><span class="sxs-lookup"><span data-stu-id="b2190-135">status</span></span>|[<span data-ttu-id="b2190-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b2190-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="b2190-137">Статус загрузки.</span><span class="sxs-lookup"><span data-stu-id="b2190-137">Upload status.</span></span> <span data-ttu-id="b2190-138">Возможные значения: `noUpload`, `pending`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="b2190-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="b2190-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2190-139">Response</span></span>
<span data-ttu-id="b2190-140">В случае успеха этот метод возвращает `201 Created` код отклика и объект [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2190-140">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2190-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b2190-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2190-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2190-142">Request</span></span>
<span data-ttu-id="b2190-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2190-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="b2190-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2190-144">Response</span></span>
<span data-ttu-id="b2190-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2190-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```








