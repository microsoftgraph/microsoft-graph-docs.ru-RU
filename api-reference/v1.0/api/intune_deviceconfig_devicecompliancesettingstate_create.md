# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="ca67d-101">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="ca67d-101">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="ca67d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ca67d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca67d-103">Создание объекта [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="ca67d-103">Create a new [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca67d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ca67d-104">Prerequisites</span></span>
<span data-ttu-id="ca67d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca67d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca67d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca67d-107">Permission type</span></span>|<span data-ttu-id="ca67d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca67d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca67d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca67d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ca67d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca67d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca67d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca67d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca67d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca67d-112">Not supported.</span></span>|
|<span data-ttu-id="ca67d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca67d-113">Application</span></span>|<span data-ttu-id="ca67d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca67d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca67d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca67d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="ca67d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca67d-116">Request headers</span></span>
|<span data-ttu-id="ca67d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca67d-117">Header</span></span>|<span data-ttu-id="ca67d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ca67d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca67d-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca67d-119">Authorization</span></span>|<span data-ttu-id="ca67d-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ca67d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca67d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ca67d-121">Accept</span></span>|<span data-ttu-id="ca67d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ca67d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca67d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca67d-123">Request body</span></span>
<span data-ttu-id="ca67d-124">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca67d-124">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="ca67d-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="ca67d-125">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="ca67d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca67d-126">Property</span></span>|<span data-ttu-id="ca67d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ca67d-127">Type</span></span>|<span data-ttu-id="ca67d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ca67d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca67d-129">id</span><span class="sxs-lookup"><span data-stu-id="ca67d-129">id</span></span>|<span data-ttu-id="ca67d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-130">String</span></span>|<span data-ttu-id="ca67d-131">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="ca67d-131">Key of the entity</span></span>|
|<span data-ttu-id="ca67d-132">setting</span><span class="sxs-lookup"><span data-stu-id="ca67d-132">setting</span></span>|<span data-ttu-id="ca67d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-133">String</span></span>|<span data-ttu-id="ca67d-134">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="ca67d-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="ca67d-135">settingName</span><span class="sxs-lookup"><span data-stu-id="ca67d-135">settingName</span></span>|<span data-ttu-id="ca67d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-136">String</span></span>|<span data-ttu-id="ca67d-137">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="ca67d-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="ca67d-138">deviceId</span></span>|<span data-ttu-id="ca67d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-139">String</span></span>|<span data-ttu-id="ca67d-140">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="ca67d-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="ca67d-141">deviceName</span></span>|<span data-ttu-id="ca67d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-142">String</span></span>|<span data-ttu-id="ca67d-143">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="ca67d-144">userId</span><span class="sxs-lookup"><span data-stu-id="ca67d-144">userId</span></span>|<span data-ttu-id="ca67d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-145">String</span></span>|<span data-ttu-id="ca67d-146">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="ca67d-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="ca67d-147">userEmail</span></span>|<span data-ttu-id="ca67d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-148">String</span></span>|<span data-ttu-id="ca67d-149">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="ca67d-150">userName</span><span class="sxs-lookup"><span data-stu-id="ca67d-150">userName</span></span>|<span data-ttu-id="ca67d-151">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-151">String</span></span>|<span data-ttu-id="ca67d-152">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="ca67d-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca67d-153">userPrincipalName</span></span>|<span data-ttu-id="ca67d-154">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-154">String</span></span>|<span data-ttu-id="ca67d-155">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="ca67d-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ca67d-156">deviceModel</span></span>|<span data-ttu-id="ca67d-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ca67d-157">String</span></span>|<span data-ttu-id="ca67d-158">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="ca67d-158">The device model that is being reported</span></span>|
|<span data-ttu-id="ca67d-159">state</span><span class="sxs-lookup"><span data-stu-id="ca67d-159">state</span></span>|[<span data-ttu-id="ca67d-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ca67d-160">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="ca67d-161">Состояние соответствия параметра.</span><span class="sxs-lookup"><span data-stu-id="ca67d-161">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="ca67d-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="ca67d-162">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="ca67d-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ca67d-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ca67d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca67d-164">DateTimeOffset</span></span>|<span data-ttu-id="ca67d-165">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ca67d-165">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="ca67d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca67d-166">Response</span></span>
<span data-ttu-id="ca67d-167">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca67d-167">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune_deviceconfig_devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca67d-168">Пример</span><span class="sxs-lookup"><span data-stu-id="ca67d-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca67d-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca67d-169">Request</span></span>
<span data-ttu-id="ca67d-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca67d-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="ca67d-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca67d-171">Response</span></span>
<span data-ttu-id="ca67d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca67d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



