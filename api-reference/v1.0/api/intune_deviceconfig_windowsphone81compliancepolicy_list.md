# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="fd000-101">Перечисление объектов windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fd000-101">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="fd000-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd000-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd000-103">Список свойств и связей объектов [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd000-103">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd000-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd000-104">Prerequisites</span></span>
<span data-ttu-id="fd000-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd000-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd000-107">Permission type</span></span>|<span data-ttu-id="fd000-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd000-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd000-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd000-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd000-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd000-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd000-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd000-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd000-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd000-112">Not supported.</span></span>|
|<span data-ttu-id="fd000-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd000-113">Application</span></span>|<span data-ttu-id="fd000-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd000-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd000-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd000-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="fd000-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd000-116">Request headers</span></span>
|<span data-ttu-id="fd000-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd000-117">Header</span></span>|<span data-ttu-id="fd000-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fd000-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd000-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd000-119">Authorization</span></span>|<span data-ttu-id="fd000-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd000-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd000-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fd000-121">Accept</span></span>|<span data-ttu-id="fd000-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fd000-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd000-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd000-123">Request body</span></span>
<span data-ttu-id="fd000-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd000-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd000-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd000-125">Response</span></span>
<span data-ttu-id="fd000-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd000-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd000-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fd000-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd000-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd000-128">Request</span></span>
<span data-ttu-id="fd000-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd000-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="fd000-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd000-130">Response</span></span>
<span data-ttu-id="fd000-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fd000-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



