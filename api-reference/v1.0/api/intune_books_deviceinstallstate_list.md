# <a name="list-deviceinstallstates"></a><span data-ttu-id="4bb92-101">Перечисление объектов deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="4bb92-101">List deviceInstallStates</span></span>

> <span data-ttu-id="4bb92-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bb92-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bb92-103">Список свойств и связей объектов [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="4bb92-103">List properties and relationships of the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bb92-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4bb92-104">Prerequisites</span></span>
<span data-ttu-id="4bb92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bb92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bb92-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bb92-107">Permission type</span></span>|<span data-ttu-id="4bb92-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bb92-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bb92-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bb92-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4bb92-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bb92-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4bb92-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bb92-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bb92-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb92-112">Not supported.</span></span>|
|<span data-ttu-id="4bb92-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bb92-113">Application</span></span>|<span data-ttu-id="4bb92-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bb92-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bb92-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bb92-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="4bb92-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bb92-116">Request headers</span></span>
|<span data-ttu-id="4bb92-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bb92-117">Header</span></span>|<span data-ttu-id="4bb92-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4bb92-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bb92-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4bb92-119">Authorization</span></span>|<span data-ttu-id="4bb92-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="4bb92-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bb92-121">Принять</span><span class="sxs-lookup"><span data-stu-id="4bb92-121">Accept</span></span>|<span data-ttu-id="4bb92-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4bb92-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bb92-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bb92-123">Request body</span></span>
<span data-ttu-id="4bb92-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bb92-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bb92-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bb92-125">Response</span></span>
<span data-ttu-id="4bb92-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceInstallState](../resources/intune_books_deviceinstallstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bb92-126">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune_books_deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bb92-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4bb92-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bb92-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bb92-128">Request</span></span>
<span data-ttu-id="4bb92-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bb92-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="4bb92-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bb92-130">Response</span></span>
<span data-ttu-id="4bb92-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bb92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```








