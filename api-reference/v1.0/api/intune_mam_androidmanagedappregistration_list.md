# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="4d3d2-101">Перечисление объектов androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="4d3d2-101">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="4d3d2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d3d2-103">Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4d3d2-103">List properties and relationships of the [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d3d2-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d3d2-104">Prerequisites</span></span>
<span data-ttu-id="4d3d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d3d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4d3d2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d3d2-107">Permission type</span></span>|<span data-ttu-id="4d3d2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d3d2-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d3d2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d3d2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4d3d2-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d3d2-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d3d2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d3d2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d3d2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-112">Not supported.</span></span>|
|<span data-ttu-id="4d3d2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d3d2-113">Application</span></span>|<span data-ttu-id="4d3d2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d3d2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d3d2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="4d3d2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d3d2-116">Request headers</span></span>
|<span data-ttu-id="4d3d2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d3d2-117">Header</span></span>|<span data-ttu-id="4d3d2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4d3d2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d3d2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d3d2-119">Authorization</span></span>|<span data-ttu-id="4d3d2-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d3d2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4d3d2-121">Accept</span></span>|<span data-ttu-id="4d3d2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4d3d2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d3d2-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d3d2-123">Request body</span></span>
<span data-ttu-id="4d3d2-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d3d2-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d3d2-125">Response</span></span>
<span data-ttu-id="4d3d2-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_mam_androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d3d2-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4d3d2-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d3d2-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d3d2-128">Request</span></span>
<span data-ttu-id="4d3d2-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="4d3d2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d3d2-130">Response</span></span>
<span data-ttu-id="4d3d2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d3d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```



