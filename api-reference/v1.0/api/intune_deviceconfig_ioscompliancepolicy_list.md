# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="ac470-101">Перечисление объектов iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ac470-101">List iosCompliancePolicies</span></span>

> <span data-ttu-id="ac470-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac470-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac470-103">Список свойств и связей объектов [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ac470-103">List properties and relationships of the [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac470-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac470-104">Prerequisites</span></span>
<span data-ttu-id="ac470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac470-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac470-107">Permission type</span></span>|<span data-ttu-id="ac470-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac470-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac470-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac470-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac470-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac470-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ac470-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac470-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac470-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac470-112">Not supported.</span></span>|
|<span data-ttu-id="ac470-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac470-113">Application</span></span>|<span data-ttu-id="ac470-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac470-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac470-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac470-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ac470-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac470-116">Request headers</span></span>
|<span data-ttu-id="ac470-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac470-117">Header</span></span>|<span data-ttu-id="ac470-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ac470-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac470-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac470-119">Authorization</span></span>|<span data-ttu-id="ac470-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ac470-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac470-121">Принять</span><span class="sxs-lookup"><span data-stu-id="ac470-121">Accept</span></span>|<span data-ttu-id="ac470-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac470-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac470-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac470-123">Request body</span></span>
<span data-ttu-id="ac470-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac470-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac470-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac470-125">Response</span></span>
<span data-ttu-id="ac470-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac470-126">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac470-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ac470-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac470-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac470-128">Request</span></span>
<span data-ttu-id="ac470-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac470-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="ac470-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac470-130">Response</span></span>
<span data-ttu-id="ac470-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```








