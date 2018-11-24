# <a name="list-detectedapps"></a><span data-ttu-id="35865-101">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="35865-101">List detectedApps</span></span>

> <span data-ttu-id="35865-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35865-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35865-103">Список свойств и связей объектов [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="35865-103">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35865-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="35865-104">Prerequisites</span></span>
<span data-ttu-id="35865-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="35865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35865-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35865-107">Permission type</span></span>|<span data-ttu-id="35865-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35865-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35865-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35865-109">Delegated (work or school account)</span></span>|<span data-ttu-id="35865-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="35865-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="35865-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35865-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35865-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35865-112">Not supported.</span></span>|
|<span data-ttu-id="35865-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35865-113">Application</span></span>|<span data-ttu-id="35865-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35865-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35865-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35865-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="35865-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35865-116">Request headers</span></span>
|<span data-ttu-id="35865-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35865-117">Header</span></span>|<span data-ttu-id="35865-118">Значение</span><span class="sxs-lookup"><span data-stu-id="35865-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35865-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="35865-119">Authorization</span></span>|<span data-ttu-id="35865-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35865-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35865-121">Accept</span><span class="sxs-lookup"><span data-stu-id="35865-121">Accept</span></span>|<span data-ttu-id="35865-122">application/json</span><span class="sxs-lookup"><span data-stu-id="35865-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35865-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35865-123">Request body</span></span>
<span data-ttu-id="35865-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35865-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35865-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="35865-125">Response</span></span>
<span data-ttu-id="35865-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune_devices_detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35865-126">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune_devices_detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35865-127">Пример</span><span class="sxs-lookup"><span data-stu-id="35865-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="35865-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="35865-128">Request</span></span>
<span data-ttu-id="35865-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35865-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="35865-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="35865-130">Response</span></span>
<span data-ttu-id="35865-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35865-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```



