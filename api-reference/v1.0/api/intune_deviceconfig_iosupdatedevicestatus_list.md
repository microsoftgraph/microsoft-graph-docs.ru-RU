# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="24f19-101">Перечисление объектов iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24f19-101">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="24f19-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="24f19-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24f19-103">Список свойств и связей объектов [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="24f19-103">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24f19-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24f19-104">Prerequisites</span></span>
<span data-ttu-id="24f19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24f19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24f19-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24f19-107">Permission type</span></span>|<span data-ttu-id="24f19-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24f19-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24f19-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24f19-109">Delegated (work or school account)</span></span>|<span data-ttu-id="24f19-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24f19-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24f19-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24f19-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24f19-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24f19-112">Not supported.</span></span>|
|<span data-ttu-id="24f19-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24f19-113">Application</span></span>|<span data-ttu-id="24f19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24f19-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24f19-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24f19-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="24f19-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24f19-116">Request headers</span></span>
|<span data-ttu-id="24f19-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24f19-117">Header</span></span>|<span data-ttu-id="24f19-118">Значение</span><span class="sxs-lookup"><span data-stu-id="24f19-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24f19-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="24f19-119">Authorization</span></span>|<span data-ttu-id="24f19-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24f19-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24f19-121">Accept</span><span class="sxs-lookup"><span data-stu-id="24f19-121">Accept</span></span>|<span data-ttu-id="24f19-122">application/json</span><span class="sxs-lookup"><span data-stu-id="24f19-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24f19-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24f19-123">Request body</span></span>
<span data-ttu-id="24f19-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24f19-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24f19-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="24f19-125">Response</span></span>
<span data-ttu-id="24f19-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24f19-126">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/intune_deviceconfig_iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24f19-127">Пример</span><span class="sxs-lookup"><span data-stu-id="24f19-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="24f19-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="24f19-128">Request</span></span>
<span data-ttu-id="24f19-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24f19-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="24f19-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="24f19-130">Response</span></span>
<span data-ttu-id="24f19-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="24f19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



