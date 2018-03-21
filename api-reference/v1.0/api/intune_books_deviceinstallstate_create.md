# <a name="create-deviceinstallstate"></a><span data-ttu-id="96182-101">Создание объекта deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="96182-101">Create deviceInstallState</span></span>

> <span data-ttu-id="96182-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96182-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96182-103">Создание объекта [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="96182-103">Create a new [plannerBucket](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96182-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="96182-104">Prerequisites</span></span>
<span data-ttu-id="96182-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96182-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96182-107">Permission type</span></span>|<span data-ttu-id="96182-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96182-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96182-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96182-109">Delegated (work or school account)</span></span>|<span data-ttu-id="96182-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96182-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96182-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96182-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96182-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96182-112">Not supported.</span></span>|
|<span data-ttu-id="96182-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96182-113">Application</span></span>|<span data-ttu-id="96182-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96182-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96182-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96182-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="96182-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96182-116">Request headers</span></span>
|<span data-ttu-id="96182-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96182-117">Header</span></span>|<span data-ttu-id="96182-118">Значение</span><span class="sxs-lookup"><span data-stu-id="96182-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96182-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="96182-119">Authorization</span></span>|<span data-ttu-id="96182-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96182-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="96182-121">Accept</span><span class="sxs-lookup"><span data-stu-id="96182-121">Accept</span></span>|<span data-ttu-id="96182-122">application/json</span><span class="sxs-lookup"><span data-stu-id="96182-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96182-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96182-123">Request body</span></span>
<span data-ttu-id="96182-124">В тексте запроса добавьте представление объекта deviceInstallState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96182-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="96182-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceInstallState.</span><span class="sxs-lookup"><span data-stu-id="96182-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="96182-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="96182-126">Property</span></span>|<span data-ttu-id="96182-127">Тип</span><span class="sxs-lookup"><span data-stu-id="96182-127">Type</span></span>|<span data-ttu-id="96182-128">Описание</span><span class="sxs-lookup"><span data-stu-id="96182-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96182-129">id</span><span class="sxs-lookup"><span data-stu-id="96182-129">id</span></span>|<span data-ttu-id="96182-130">String</span><span class="sxs-lookup"><span data-stu-id="96182-130">String</span></span>|<span data-ttu-id="96182-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96182-131">Key of the setting.</span></span>|
|<span data-ttu-id="96182-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="96182-132">deviceName</span></span>|<span data-ttu-id="96182-133">String</span><span class="sxs-lookup"><span data-stu-id="96182-133">String</span></span>|<span data-ttu-id="96182-134">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="96182-134">Device name.</span></span>|
|<span data-ttu-id="96182-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="96182-135">deviceId</span></span>|<span data-ttu-id="96182-136">String</span><span class="sxs-lookup"><span data-stu-id="96182-136">String</span></span>|<span data-ttu-id="96182-137">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="96182-137">Device Id.</span></span>|
|<span data-ttu-id="96182-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="96182-138">lastSyncDateTime</span></span>|<span data-ttu-id="96182-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96182-139">DateTimeOffset</span></span>|<span data-ttu-id="96182-140">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96182-140">Last sync date and time.</span></span>|
|<span data-ttu-id="96182-141">installState</span><span class="sxs-lookup"><span data-stu-id="96182-141">installState</span></span>|<span data-ttu-id="96182-142">String</span><span class="sxs-lookup"><span data-stu-id="96182-142">String</span></span>|<span data-ttu-id="96182-143">Состояние установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="96182-143">The install state of the eBook.</span></span> <span data-ttu-id="96182-144">Возможные значения: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="96182-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="96182-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="96182-145">errorCode</span></span>|<span data-ttu-id="96182-146">String</span><span class="sxs-lookup"><span data-stu-id="96182-146">String</span></span>|<span data-ttu-id="96182-147">Код ошибки для сбоев при установке.</span><span class="sxs-lookup"><span data-stu-id="96182-147">The error code for install failures.</span></span>|
|<span data-ttu-id="96182-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="96182-148">osVersion</span></span>|<span data-ttu-id="96182-149">String</span><span class="sxs-lookup"><span data-stu-id="96182-149">String</span></span>|<span data-ttu-id="96182-150">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="96182-150">OS Version.</span></span>|
|<span data-ttu-id="96182-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="96182-151">osDescription</span></span>|<span data-ttu-id="96182-152">String</span><span class="sxs-lookup"><span data-stu-id="96182-152">String</span></span>|<span data-ttu-id="96182-153">Описание ОС.</span><span class="sxs-lookup"><span data-stu-id="96182-153">OS Description.</span></span>|
|<span data-ttu-id="96182-154">userName</span><span class="sxs-lookup"><span data-stu-id="96182-154">userName</span></span>|<span data-ttu-id="96182-155">String</span><span class="sxs-lookup"><span data-stu-id="96182-155">String</span></span>|<span data-ttu-id="96182-156">Имя пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="96182-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="96182-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="96182-157">Response</span></span>
<span data-ttu-id="96182-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceInstallState](../resources/intune_books_deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96182-158">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96182-159">Пример</span><span class="sxs-lookup"><span data-stu-id="96182-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="96182-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="96182-160">Request</span></span>
<span data-ttu-id="96182-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96182-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="96182-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="96182-162">Response</span></span>
<span data-ttu-id="96182-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96182-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```



