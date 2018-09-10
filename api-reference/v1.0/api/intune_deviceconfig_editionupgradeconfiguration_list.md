# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="dbfa3-101">Перечисление объектов editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="dbfa3-101">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="dbfa3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbfa3-103">Список свойств и связей объектов [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dbfa3-103">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbfa3-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dbfa3-104">Prerequisites</span></span>
<span data-ttu-id="dbfa3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dbfa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dbfa3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbfa3-107">Permission type</span></span>|<span data-ttu-id="dbfa3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbfa3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbfa3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbfa3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dbfa3-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbfa3-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbfa3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbfa3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbfa3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-112">Not supported.</span></span>|
|<span data-ttu-id="dbfa3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbfa3-113">Application</span></span>|<span data-ttu-id="dbfa3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbfa3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbfa3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dbfa3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbfa3-116">Request headers</span></span>
|<span data-ttu-id="dbfa3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbfa3-117">Header</span></span>|<span data-ttu-id="dbfa3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="dbfa3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbfa3-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbfa3-119">Authorization</span></span>|<span data-ttu-id="dbfa3-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="dbfa3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbfa3-121">Принять</span><span class="sxs-lookup"><span data-stu-id="dbfa3-121">Accept</span></span>|<span data-ttu-id="dbfa3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dbfa3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbfa3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbfa3-123">Request body</span></span>
<span data-ttu-id="dbfa3-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbfa3-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbfa3-125">Response</span></span>
<span data-ttu-id="dbfa3-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-126">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbfa3-127">Пример</span><span class="sxs-lookup"><span data-stu-id="dbfa3-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbfa3-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbfa3-128">Request</span></span>
<span data-ttu-id="dbfa3-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dbfa3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dbfa3-130">Response</span></span>
<span data-ttu-id="dbfa3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbfa3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "licenseFile",
      "targetEdition": "windows10EnterpriseN",
      "license": "License value",
      "productKey": "Product Key value"
    }
  ]
}
```








