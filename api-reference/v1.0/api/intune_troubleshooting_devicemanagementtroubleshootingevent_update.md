# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="56873-101">Обновление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="56873-101">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="56873-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56873-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56873-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56873-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56873-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56873-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56873-105">Обновление свойств объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="56873-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56873-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="56873-106">Prerequisites</span></span>
<span data-ttu-id="56873-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56873-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="56873-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56873-109">Permission type</span></span>|<span data-ttu-id="56873-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56873-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56873-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56873-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56873-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56873-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56873-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56873-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56873-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56873-114">Not supported.</span></span>|
|<span data-ttu-id="56873-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56873-115">Application</span></span>|<span data-ttu-id="56873-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56873-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56873-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56873-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="56873-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="56873-118">Request headers</span></span>
|<span data-ttu-id="56873-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56873-119">Header</span></span>|<span data-ttu-id="56873-120">Значение</span><span class="sxs-lookup"><span data-stu-id="56873-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56873-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56873-121">Authorization</span></span>|<span data-ttu-id="56873-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56873-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56873-123">Accept</span><span class="sxs-lookup"><span data-stu-id="56873-123">Accept</span></span>|<span data-ttu-id="56873-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56873-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56873-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56873-125">Request body</span></span>
<span data-ttu-id="56873-126">В теле запроса добавьте представление объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56873-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="56873-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="56873-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="56873-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="56873-128">Property</span></span>|<span data-ttu-id="56873-129">Тип</span><span class="sxs-lookup"><span data-stu-id="56873-129">Type</span></span>|<span data-ttu-id="56873-130">Описание</span><span class="sxs-lookup"><span data-stu-id="56873-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56873-131">id</span><span class="sxs-lookup"><span data-stu-id="56873-131">id</span></span>|<span data-ttu-id="56873-132">String</span><span class="sxs-lookup"><span data-stu-id="56873-132">String</span></span>|<span data-ttu-id="56873-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="56873-133">UUID for the object</span></span>|
|<span data-ttu-id="56873-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="56873-134">eventDateTime</span></span>|<span data-ttu-id="56873-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56873-135">DateTimeOffset</span></span>|<span data-ttu-id="56873-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="56873-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="56873-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="56873-137">correlationId</span></span>|<span data-ttu-id="56873-138">String</span><span class="sxs-lookup"><span data-stu-id="56873-138">String</span></span>|<span data-ttu-id="56873-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="56873-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="56873-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="56873-140">Response</span></span>
<span data-ttu-id="56873-141">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="56873-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56873-142">Пример</span><span class="sxs-lookup"><span data-stu-id="56873-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="56873-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="56873-143">Request</span></span>
<span data-ttu-id="56873-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56873-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 104

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="56873-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="56873-145">Response</span></span>
<span data-ttu-id="56873-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56873-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



