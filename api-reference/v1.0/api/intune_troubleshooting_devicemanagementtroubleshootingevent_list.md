# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="ec40a-101">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ec40a-101">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="ec40a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ec40a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec40a-103">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ec40a-103">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec40a-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec40a-104">Prerequisites</span></span>
<span data-ttu-id="ec40a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ec40a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec40a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec40a-107">Permission type</span></span>|<span data-ttu-id="ec40a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec40a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec40a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec40a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec40a-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec40a-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ec40a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec40a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec40a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec40a-112">Not supported.</span></span>|
|<span data-ttu-id="ec40a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec40a-113">Application</span></span>|<span data-ttu-id="ec40a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec40a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec40a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec40a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ec40a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec40a-116">Request headers</span></span>
|<span data-ttu-id="ec40a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec40a-117">Header</span></span>|<span data-ttu-id="ec40a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ec40a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec40a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec40a-119">Authorization</span></span>|<span data-ttu-id="ec40a-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ec40a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec40a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ec40a-121">Accept</span></span>|<span data-ttu-id="ec40a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ec40a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec40a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec40a-123">Request body</span></span>
<span data-ttu-id="ec40a-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec40a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec40a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec40a-125">Response</span></span>
<span data-ttu-id="ec40a-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec40a-126">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec40a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ec40a-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec40a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec40a-128">Request</span></span>
<span data-ttu-id="ec40a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec40a-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="ec40a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec40a-130">Response</span></span>
<span data-ttu-id="ec40a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ec40a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```



