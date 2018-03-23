# <a name="update-devicecompliancepolicystate"></a><span data-ttu-id="a39cc-101">Обновление объекта deviceCompliancePolicyState</span><span class="sxs-lookup"><span data-stu-id="a39cc-101">Update deviceCompliancePolicyState</span></span>

> <span data-ttu-id="a39cc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a39cc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a39cc-103">Обновление свойств объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).</span><span class="sxs-lookup"><span data-stu-id="a39cc-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a39cc-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a39cc-104">Prerequisites</span></span>
<span data-ttu-id="a39cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a39cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a39cc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a39cc-107">Permission type</span></span>|<span data-ttu-id="a39cc-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a39cc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a39cc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a39cc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a39cc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a39cc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a39cc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a39cc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a39cc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a39cc-112">Not supported.</span></span>|
|<span data-ttu-id="a39cc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a39cc-113">Application</span></span>|<span data-ttu-id="a39cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a39cc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a39cc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a39cc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a39cc-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a39cc-116">Request headers</span></span>
|<span data-ttu-id="a39cc-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a39cc-117">Header</span></span>|<span data-ttu-id="a39cc-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a39cc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a39cc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a39cc-119">Authorization</span></span>|<span data-ttu-id="a39cc-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a39cc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a39cc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a39cc-121">Accept</span></span>|<span data-ttu-id="a39cc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a39cc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a39cc-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a39cc-123">Request body</span></span>
<span data-ttu-id="a39cc-124">В теле запроса добавьте представление объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a39cc-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>

<span data-ttu-id="a39cc-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).</span><span class="sxs-lookup"><span data-stu-id="a39cc-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a39cc-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a39cc-126">Property</span></span>|<span data-ttu-id="a39cc-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a39cc-127">Type</span></span>|<span data-ttu-id="a39cc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a39cc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a39cc-129">id</span><span class="sxs-lookup"><span data-stu-id="a39cc-129">id</span></span>|<span data-ttu-id="a39cc-130">String</span><span class="sxs-lookup"><span data-stu-id="a39cc-130">String</span></span>|<span data-ttu-id="a39cc-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a39cc-131">Key of the setting.</span></span>|
|<span data-ttu-id="a39cc-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="a39cc-132">settingStates</span></span>|<span data-ttu-id="a39cc-133">Коллекция [deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="a39cc-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) collection</span></span>|<span data-ttu-id="a39cc-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a39cc-134">Not yet documented</span></span>|
|<span data-ttu-id="a39cc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a39cc-135">displayName</span></span>|<span data-ttu-id="a39cc-136">String</span><span class="sxs-lookup"><span data-stu-id="a39cc-136">String</span></span>|<span data-ttu-id="a39cc-137">Имя политики для policyBase.</span><span class="sxs-lookup"><span data-stu-id="a39cc-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="a39cc-138">version</span><span class="sxs-lookup"><span data-stu-id="a39cc-138">version</span></span>|<span data-ttu-id="a39cc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a39cc-139">Int32</span></span>|<span data-ttu-id="a39cc-140">Версия политики.</span><span class="sxs-lookup"><span data-stu-id="a39cc-140">The version of the message.</span></span>|
|<span data-ttu-id="a39cc-141">platformType</span><span class="sxs-lookup"><span data-stu-id="a39cc-141">PlatformType</span></span>|<span data-ttu-id="a39cc-142">String</span><span class="sxs-lookup"><span data-stu-id="a39cc-142">String</span></span>|<span data-ttu-id="a39cc-143">Тип платформы, к которой относится политика. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a39cc-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="a39cc-144">state</span><span class="sxs-lookup"><span data-stu-id="a39cc-144">state</span></span>|<span data-ttu-id="a39cc-145">String</span><span class="sxs-lookup"><span data-stu-id="a39cc-145">String</span></span>|<span data-ttu-id="a39cc-146">Состояние соответствия требованиям для политики. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="a39cc-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="a39cc-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="a39cc-147">settingCount</span></span>|<span data-ttu-id="a39cc-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a39cc-148">Int32</span></span>|<span data-ttu-id="a39cc-149">Количество параметров в политике.</span><span class="sxs-lookup"><span data-stu-id="a39cc-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="a39cc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a39cc-150">Response</span></span>
<span data-ttu-id="a39cc-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a39cc-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a39cc-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a39cc-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="a39cc-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a39cc-153">Request</span></span>
<span data-ttu-id="a39cc-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a39cc-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
Content-type: application/json
Content-length: 907

{
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```

### <a name="response"></a><span data-ttu-id="a39cc-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="a39cc-155">Response</span></span>
<span data-ttu-id="a39cc-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a39cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1022

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "2999e387-e387-2999-87e3-992987e39929",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "notApplicable",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "iOS",
  "state": "notApplicable",
  "settingCount": 12
}
```



