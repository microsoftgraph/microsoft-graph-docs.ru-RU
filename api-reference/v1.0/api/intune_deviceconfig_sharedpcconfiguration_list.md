# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="79f5e-101">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="79f5e-101">List sharedPCConfigurations</span></span>

> <span data-ttu-id="79f5e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79f5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79f5e-103">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="79f5e-103">List properties and relationships of the [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79f5e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79f5e-104">Prerequisites</span></span>
<span data-ttu-id="79f5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79f5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79f5e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f5e-107">Permission type</span></span>|<span data-ttu-id="79f5e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f5e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79f5e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f5e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79f5e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79f5e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79f5e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f5e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f5e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f5e-112">Not supported.</span></span>|
|<span data-ttu-id="79f5e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79f5e-113">Application</span></span>|<span data-ttu-id="79f5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f5e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79f5e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79f5e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79f5e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79f5e-116">Request headers</span></span>
|<span data-ttu-id="79f5e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79f5e-117">Header</span></span>|<span data-ttu-id="79f5e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="79f5e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79f5e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="79f5e-119">Authorization</span></span>|<span data-ttu-id="79f5e-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79f5e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79f5e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="79f5e-121">Accept</span></span>|<span data-ttu-id="79f5e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="79f5e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f5e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79f5e-123">Request body</span></span>
<span data-ttu-id="79f5e-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79f5e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79f5e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f5e-125">Response</span></span>
<span data-ttu-id="79f5e-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79f5e-126">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune_deviceconfig_sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f5e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="79f5e-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="79f5e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f5e-128">Request</span></span>
<span data-ttu-id="79f5e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f5e-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="79f5e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="79f5e-130">Response</span></span>
<span data-ttu-id="79f5e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79f5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1165

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedPCConfiguration",
      "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountManagerPolicy": {
        "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
        "accountDeletionPolicy": "diskSpaceThreshold",
        "cacheAccountsAboveDiskFreePercentage": 4,
        "inactiveThresholdDays": 5,
        "removeAccountsBelowDiskFreePercentage": 5
      },
      "allowedAccounts": "domain",
      "allowLocalStorage": true,
      "disableAccountManager": true,
      "disableEduPolicies": true,
      "disablePowerPolicies": true,
      "disableSignInOnResume": true,
      "enabled": true,
      "idleTimeBeforeSleepInSeconds": 12,
      "kioskAppDisplayName": "Kiosk App Display Name value",
      "kioskAppUserModelId": "Kiosk App User Model Id value",
      "maintenanceStartTime": "11:59:24.7240000"
    }
  ]
}
```



