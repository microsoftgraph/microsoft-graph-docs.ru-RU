# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="beaf6-101">Создание объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="beaf6-101">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="beaf6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="beaf6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beaf6-103">Создание объекта [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="beaf6-103">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beaf6-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="beaf6-104">Prerequisites</span></span>
<span data-ttu-id="beaf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="beaf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="beaf6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="beaf6-107">Permission type</span></span>|<span data-ttu-id="beaf6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="beaf6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beaf6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="beaf6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="beaf6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beaf6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="beaf6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="beaf6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beaf6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beaf6-112">Not supported.</span></span>|
|<span data-ttu-id="beaf6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="beaf6-113">Application</span></span>|<span data-ttu-id="beaf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="beaf6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beaf6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="beaf6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="beaf6-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="beaf6-116">Request headers</span></span>
|<span data-ttu-id="beaf6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="beaf6-117">Header</span></span>|<span data-ttu-id="beaf6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="beaf6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beaf6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="beaf6-119">Authorization</span></span>|<span data-ttu-id="beaf6-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="beaf6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="beaf6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="beaf6-121">Accept</span></span>|<span data-ttu-id="beaf6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="beaf6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beaf6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="beaf6-123">Request body</span></span>
<span data-ttu-id="beaf6-124">В тексте запроса добавьте представление объекта deviceConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beaf6-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="beaf6-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="beaf6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="beaf6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="beaf6-126">Property</span></span>|<span data-ttu-id="beaf6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="beaf6-127">Type</span></span>|<span data-ttu-id="beaf6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="beaf6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beaf6-129">id</span><span class="sxs-lookup"><span data-stu-id="beaf6-129">id</span></span>|<span data-ttu-id="beaf6-130">String</span><span class="sxs-lookup"><span data-stu-id="beaf6-130">String</span></span>|<span data-ttu-id="beaf6-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="beaf6-131">Key of the setting.</span></span>|
|<span data-ttu-id="beaf6-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="beaf6-132">userDisplayName</span></span>|<span data-ttu-id="beaf6-133">String</span><span class="sxs-lookup"><span data-stu-id="beaf6-133">String</span></span>|<span data-ttu-id="beaf6-134">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="beaf6-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="beaf6-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="beaf6-135">devicesCount</span></span>|<span data-ttu-id="beaf6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="beaf6-136">Int32</span></span>|<span data-ttu-id="beaf6-137">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="beaf6-137">Devices count for that user.</span></span>|
|<span data-ttu-id="beaf6-138">status</span><span class="sxs-lookup"><span data-stu-id="beaf6-138">status</span></span>|<span data-ttu-id="beaf6-139">String</span><span class="sxs-lookup"><span data-stu-id="beaf6-139">String</span></span>|<span data-ttu-id="beaf6-140">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="beaf6-140">Compliance status of the policy report.</span></span> <span data-ttu-id="beaf6-141">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="beaf6-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="beaf6-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="beaf6-142">lastReportedDateTime</span></span>|<span data-ttu-id="beaf6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beaf6-143">DateTimeOffset</span></span>|<span data-ttu-id="beaf6-144">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="beaf6-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="beaf6-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="beaf6-145">userPrincipalName</span></span>|<span data-ttu-id="beaf6-146">String</span><span class="sxs-lookup"><span data-stu-id="beaf6-146">String</span></span>|<span data-ttu-id="beaf6-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="beaf6-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="beaf6-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="beaf6-148">Response</span></span>
<span data-ttu-id="beaf6-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="beaf6-149">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beaf6-150">Пример</span><span class="sxs-lookup"><span data-stu-id="beaf6-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="beaf6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="beaf6-151">Request</span></span>
<span data-ttu-id="beaf6-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="beaf6-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="beaf6-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="beaf6-153">Response</span></span>
<span data-ttu-id="beaf6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="beaf6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



