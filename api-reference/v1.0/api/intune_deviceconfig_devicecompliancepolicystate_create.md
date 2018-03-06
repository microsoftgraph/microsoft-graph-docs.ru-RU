# <a name="create-devicecompliancepolicystate"></a><span data-ttu-id="b5b06-101">Create deviceCompliancePolicyState</span><span class="sxs-lookup"><span data-stu-id="b5b06-101">Create deviceCompliancePolicyState</span></span>

> <span data-ttu-id="b5b06-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b5b06-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5b06-103">Создание объекта [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).</span><span class="sxs-lookup"><span data-stu-id="b5b06-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5b06-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b5b06-104">Prerequisites</span></span>
<span data-ttu-id="b5b06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5b06-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5b06-107">Permission type</span></span>|<span data-ttu-id="b5b06-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5b06-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5b06-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5b06-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b5b06-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b06-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5b06-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5b06-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5b06-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5b06-112">Not supported.</span></span>|
|<span data-ttu-id="b5b06-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5b06-113">Application</span></span>|<span data-ttu-id="b5b06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5b06-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5b06-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5b06-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a><span data-ttu-id="b5b06-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5b06-116">Request headers</span></span>
|<span data-ttu-id="b5b06-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5b06-117">Header</span></span>|<span data-ttu-id="b5b06-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b5b06-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5b06-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b06-119">Authorization</span></span>|<span data-ttu-id="b5b06-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5b06-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b5b06-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b5b06-121">Accept</span></span>|<span data-ttu-id="b5b06-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b5b06-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5b06-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5b06-123">Request body</span></span>
<span data-ttu-id="b5b06-124">В теле запроса добавьте представление объекта deviceCompliancePolicyState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5b06-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b5b06-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyState.</span><span class="sxs-lookup"><span data-stu-id="b5b06-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b5b06-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5b06-126">Property</span></span>|<span data-ttu-id="b5b06-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b5b06-127">Type</span></span>|<span data-ttu-id="b5b06-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b5b06-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5b06-129">id</span><span class="sxs-lookup"><span data-stu-id="b5b06-129">id</span></span>|<span data-ttu-id="b5b06-130">String</span><span class="sxs-lookup"><span data-stu-id="b5b06-130">String</span></span>|<span data-ttu-id="b5b06-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b5b06-131">Key of the setting.</span></span>|
|<span data-ttu-id="b5b06-132">settingStates</span><span class="sxs-lookup"><span data-stu-id="b5b06-132">settingStates</span></span>|<span data-ttu-id="b5b06-133">Коллекция [deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="b5b06-133">[deviceCompliancePolicySettingState](../resources/intune_deviceconfig_devicecompliancepolicysettingstate.md) collection</span></span>|<span data-ttu-id="b5b06-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b5b06-134">Not yet documented</span></span>|
|<span data-ttu-id="b5b06-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b5b06-135">displayName</span></span>|<span data-ttu-id="b5b06-136">String</span><span class="sxs-lookup"><span data-stu-id="b5b06-136">String</span></span>|<span data-ttu-id="b5b06-137">Имя политики для этой основы</span><span class="sxs-lookup"><span data-stu-id="b5b06-137">The name of the policy for this policyBase</span></span>|
|<span data-ttu-id="b5b06-138">version</span><span class="sxs-lookup"><span data-stu-id="b5b06-138">version</span></span>|<span data-ttu-id="b5b06-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b5b06-139">Int32</span></span>|<span data-ttu-id="b5b06-140">Версия политики</span><span class="sxs-lookup"><span data-stu-id="b5b06-140">The version of the message.</span></span>|
|<span data-ttu-id="b5b06-141">platformType</span><span class="sxs-lookup"><span data-stu-id="b5b06-141">PlatformType</span></span>|<span data-ttu-id="b5b06-142">String</span><span class="sxs-lookup"><span data-stu-id="b5b06-142">String</span></span>|<span data-ttu-id="b5b06-143">Тип платформы, к которой относится политика. Возможные значения: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span><span class="sxs-lookup"><span data-stu-id="b5b06-143">Platform type that the policy applies to Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="b5b06-144">state</span><span class="sxs-lookup"><span data-stu-id="b5b06-144">state</span></span>|<span data-ttu-id="b5b06-145">String</span><span class="sxs-lookup"><span data-stu-id="b5b06-145">String</span></span>|<span data-ttu-id="b5b06-146">Состояние соответствия требованиям для политики. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="b5b06-146">The compliance state of the policy Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="b5b06-147">settingCount</span><span class="sxs-lookup"><span data-stu-id="b5b06-147">settingCount</span></span>|<span data-ttu-id="b5b06-148">Int32</span><span class="sxs-lookup"><span data-stu-id="b5b06-148">Int32</span></span>|<span data-ttu-id="b5b06-149">Количество параметров в политике</span><span class="sxs-lookup"><span data-stu-id="b5b06-149">Count of how many setting a policy holds</span></span>|



## <a name="response"></a><span data-ttu-id="b5b06-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5b06-150">Response</span></span>
<span data-ttu-id="b5b06-151">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b5b06-151">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancepolicystate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b06-152">Пример</span><span class="sxs-lookup"><span data-stu-id="b5b06-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5b06-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5b06-153">Request</span></span>
<span data-ttu-id="b5b06-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5b06-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
Content-type: application/json
Content-length: 973

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
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

### <a name="response"></a><span data-ttu-id="b5b06-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5b06-155">Response</span></span>
<span data-ttu-id="b5b06-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b5b06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



