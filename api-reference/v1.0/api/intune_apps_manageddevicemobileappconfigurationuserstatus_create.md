# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="b1009-101">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="b1009-101">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="b1009-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b1009-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1009-103">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b1009-103">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1009-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1009-104">Prerequisites</span></span>
<span data-ttu-id="b1009-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1009-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1009-107">Permission type</span></span>|<span data-ttu-id="b1009-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1009-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1009-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1009-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b1009-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1009-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1009-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1009-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1009-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1009-112">Not supported.</span></span>|
|<span data-ttu-id="b1009-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1009-113">Application</span></span>|<span data-ttu-id="b1009-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1009-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1009-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1009-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b1009-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1009-116">Request headers</span></span>
|<span data-ttu-id="b1009-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1009-117">Header</span></span>|<span data-ttu-id="b1009-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b1009-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1009-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1009-119">Authorization</span></span>|<span data-ttu-id="b1009-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1009-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1009-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b1009-121">Accept</span></span>|<span data-ttu-id="b1009-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b1009-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1009-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1009-123">Request body</span></span>
<span data-ttu-id="b1009-124">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1009-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="b1009-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="b1009-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="b1009-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1009-126">Property</span></span>|<span data-ttu-id="b1009-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b1009-127">Type</span></span>|<span data-ttu-id="b1009-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b1009-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1009-129">id</span><span class="sxs-lookup"><span data-stu-id="b1009-129">id</span></span>|<span data-ttu-id="b1009-130">String</span><span class="sxs-lookup"><span data-stu-id="b1009-130">String</span></span>|<span data-ttu-id="b1009-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1009-131">Key of the entity.</span></span>|
|<span data-ttu-id="b1009-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1009-132">userDisplayName</span></span>|<span data-ttu-id="b1009-133">String</span><span class="sxs-lookup"><span data-stu-id="b1009-133">String</span></span>|<span data-ttu-id="b1009-134">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b1009-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b1009-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b1009-135">devicesCount</span></span>|<span data-ttu-id="b1009-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b1009-136">Int32</span></span>|<span data-ttu-id="b1009-137">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1009-137">Devices count for that user.</span></span>|
|<span data-ttu-id="b1009-138">status</span><span class="sxs-lookup"><span data-stu-id="b1009-138">status</span></span>|[<span data-ttu-id="b1009-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b1009-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="b1009-140">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b1009-140">Compliance status of the policy report.</span></span> <span data-ttu-id="b1009-141">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b1009-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b1009-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1009-142">lastReportedDateTime</span></span>|<span data-ttu-id="b1009-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1009-143">DateTimeOffset</span></span>|<span data-ttu-id="b1009-144">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b1009-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b1009-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1009-145">userPrincipalName</span></span>|<span data-ttu-id="b1009-146">String</span><span class="sxs-lookup"><span data-stu-id="b1009-146">String</span></span>|<span data-ttu-id="b1009-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1009-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b1009-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1009-148">Response</span></span>
<span data-ttu-id="b1009-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1009-149">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1009-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b1009-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1009-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1009-151">Request</span></span>
<span data-ttu-id="b1009-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1009-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b1009-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1009-153">Response</span></span>
<span data-ttu-id="b1009-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b1009-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



