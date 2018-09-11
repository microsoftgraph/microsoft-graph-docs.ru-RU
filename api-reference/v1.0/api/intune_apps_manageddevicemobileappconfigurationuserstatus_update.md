# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="c464a-101">Обновление объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c464a-101">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="c464a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c464a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c464a-103">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c464a-103">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c464a-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c464a-104">Prerequisites</span></span>
<span data-ttu-id="c464a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c464a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c464a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c464a-107">Permission type</span></span>|<span data-ttu-id="c464a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c464a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c464a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c464a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c464a-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c464a-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c464a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c464a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c464a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c464a-112">Not supported.</span></span>|
|<span data-ttu-id="c464a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c464a-113">Application</span></span>|<span data-ttu-id="c464a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c464a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c464a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c464a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c464a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c464a-116">Request headers</span></span>
|<span data-ttu-id="c464a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c464a-117">Header</span></span>|<span data-ttu-id="c464a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c464a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c464a-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c464a-119">Authorization</span></span>|<span data-ttu-id="c464a-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c464a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c464a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c464a-121">Accept</span></span>|<span data-ttu-id="c464a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c464a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c464a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c464a-123">Request body</span></span>
<span data-ttu-id="c464a-124">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c464a-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="c464a-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c464a-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="c464a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c464a-126">Property</span></span>|<span data-ttu-id="c464a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c464a-127">Type</span></span>|<span data-ttu-id="c464a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c464a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c464a-129">id</span><span class="sxs-lookup"><span data-stu-id="c464a-129">id</span></span>|<span data-ttu-id="c464a-130">Строка</span><span class="sxs-lookup"><span data-stu-id="c464a-130">String</span></span>|<span data-ttu-id="c464a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c464a-131">Key of the entity.</span></span>|
|<span data-ttu-id="c464a-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c464a-132">userDisplayName</span></span>|<span data-ttu-id="c464a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c464a-133">String</span></span>|<span data-ttu-id="c464a-134">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c464a-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c464a-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c464a-135">devicesCount</span></span>|<span data-ttu-id="c464a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c464a-136">Int32</span></span>|<span data-ttu-id="c464a-137">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c464a-137">Devices count for that user.</span></span>|
|<span data-ttu-id="c464a-138">status</span><span class="sxs-lookup"><span data-stu-id="c464a-138">status</span></span>|[<span data-ttu-id="c464a-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c464a-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="c464a-p102">Состояние соответствия требованиям отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c464a-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="c464a-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c464a-142">lastReportedDateTime</span></span>|<span data-ttu-id="c464a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c464a-143">DateTimeOffset</span></span>|<span data-ttu-id="c464a-144">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="c464a-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c464a-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c464a-145">userPrincipalName</span></span>|<span data-ttu-id="c464a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c464a-146">String</span></span>|<span data-ttu-id="c464a-147">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c464a-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c464a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c464a-148">Response</span></span>
<span data-ttu-id="c464a-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c464a-149">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune_apps_manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c464a-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c464a-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="c464a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c464a-151">Request</span></span>
<span data-ttu-id="c464a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c464a-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c464a-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="c464a-153">Response</span></span>
<span data-ttu-id="c464a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c464a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








