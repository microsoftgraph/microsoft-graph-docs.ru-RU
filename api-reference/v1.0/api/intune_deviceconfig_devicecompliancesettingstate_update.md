# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="5a491-101">Обновление объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="5a491-101">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="5a491-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5a491-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a491-103">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="5a491-103">Update the properties of a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a491-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5a491-104">Prerequisites</span></span>
<span data-ttu-id="5a491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a491-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a491-107">Permission type</span></span>|<span data-ttu-id="5a491-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a491-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a491-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a491-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a491-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a491-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a491-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a491-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a491-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a491-112">Not supported.</span></span>|
|<span data-ttu-id="5a491-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a491-113">Application</span></span>|<span data-ttu-id="5a491-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a491-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a491-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a491-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5a491-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a491-116">Request headers</span></span>
|<span data-ttu-id="5a491-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a491-117">Header</span></span>|<span data-ttu-id="5a491-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5a491-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a491-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a491-119">Authorization</span></span>|<span data-ttu-id="5a491-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="5a491-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a491-121">Принять</span><span class="sxs-lookup"><span data-stu-id="5a491-121">Accept</span></span>|<span data-ttu-id="5a491-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a491-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a491-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5a491-123">Request body</span></span>
<span data-ttu-id="5a491-124">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a491-124">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="5a491-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="5a491-125">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="5a491-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a491-126">Property</span></span>|<span data-ttu-id="5a491-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5a491-127">Type</span></span>|<span data-ttu-id="5a491-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5a491-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a491-129">id</span><span class="sxs-lookup"><span data-stu-id="5a491-129">id</span></span>|<span data-ttu-id="5a491-130">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-130">String</span></span>|<span data-ttu-id="5a491-131">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="5a491-131">Key of the entity</span></span>|
|<span data-ttu-id="5a491-132">setting</span><span class="sxs-lookup"><span data-stu-id="5a491-132">setting</span></span>|<span data-ttu-id="5a491-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-133">String</span></span>|<span data-ttu-id="5a491-134">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="5a491-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="5a491-135">settingName</span><span class="sxs-lookup"><span data-stu-id="5a491-135">settingName</span></span>|<span data-ttu-id="5a491-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-136">String</span></span>|<span data-ttu-id="5a491-137">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="5a491-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="5a491-138">deviceId</span></span>|<span data-ttu-id="5a491-139">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-139">String</span></span>|<span data-ttu-id="5a491-140">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="5a491-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="5a491-141">deviceName</span></span>|<span data-ttu-id="5a491-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-142">String</span></span>|<span data-ttu-id="5a491-143">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="5a491-144">userId</span><span class="sxs-lookup"><span data-stu-id="5a491-144">userId</span></span>|<span data-ttu-id="5a491-145">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-145">String</span></span>|<span data-ttu-id="5a491-146">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="5a491-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="5a491-147">userEmail</span></span>|<span data-ttu-id="5a491-148">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-148">String</span></span>|<span data-ttu-id="5a491-149">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="5a491-150">userName</span><span class="sxs-lookup"><span data-stu-id="5a491-150">userName</span></span>|<span data-ttu-id="5a491-151">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-151">String</span></span>|<span data-ttu-id="5a491-152">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="5a491-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a491-153">userPrincipalName</span></span>|<span data-ttu-id="5a491-154">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-154">String</span></span>|<span data-ttu-id="5a491-155">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="5a491-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5a491-156">deviceModel</span></span>|<span data-ttu-id="5a491-157">Строка</span><span class="sxs-lookup"><span data-stu-id="5a491-157">String</span></span>|<span data-ttu-id="5a491-158">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="5a491-158">The device model that is being reported</span></span>|
|<span data-ttu-id="5a491-159">state</span><span class="sxs-lookup"><span data-stu-id="5a491-159">state</span></span>|[<span data-ttu-id="5a491-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5a491-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="5a491-161">Состояние соответствия параметра.</span><span class="sxs-lookup"><span data-stu-id="5a491-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="5a491-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5a491-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5a491-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5a491-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5a491-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a491-164">DateTimeOffset</span></span>|<span data-ttu-id="5a491-165">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5a491-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="5a491-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a491-166">Response</span></span>
<span data-ttu-id="5a491-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5a491-167">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a491-168">Пример</span><span class="sxs-lookup"><span data-stu-id="5a491-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a491-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a491-169">Request</span></span>
<span data-ttu-id="5a491-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a491-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 450

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5a491-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a491-171">Response</span></span>
<span data-ttu-id="5a491-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a491-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```








