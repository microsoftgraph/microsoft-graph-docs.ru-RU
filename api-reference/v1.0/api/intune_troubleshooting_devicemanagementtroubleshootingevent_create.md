# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="9143b-101">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9143b-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="9143b-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9143b-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9143b-103">Использование данных API интерфейсов в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9143b-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9143b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9143b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9143b-105">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="9143b-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9143b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9143b-106">Prerequisites</span></span>
<span data-ttu-id="9143b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9143b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9143b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9143b-109">Permission type</span></span>|<span data-ttu-id="9143b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9143b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9143b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9143b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9143b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9143b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9143b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9143b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9143b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9143b-114">Not supported.</span></span>|
|<span data-ttu-id="9143b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9143b-115">Application</span></span>|<span data-ttu-id="9143b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9143b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9143b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9143b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="9143b-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9143b-118">Request headers</span></span>
|<span data-ttu-id="9143b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9143b-119">Header</span></span>|<span data-ttu-id="9143b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9143b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9143b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9143b-121">Authorization</span></span>|<span data-ttu-id="9143b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9143b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9143b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9143b-123">Accept</span></span>|<span data-ttu-id="9143b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9143b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9143b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9143b-125">Request body</span></span>
<span data-ttu-id="9143b-126">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9143b-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="9143b-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="9143b-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="9143b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9143b-128">Property</span></span>|<span data-ttu-id="9143b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9143b-129">Type</span></span>|<span data-ttu-id="9143b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9143b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9143b-131">id</span><span class="sxs-lookup"><span data-stu-id="9143b-131">id</span></span>|<span data-ttu-id="9143b-132">String</span><span class="sxs-lookup"><span data-stu-id="9143b-132">String</span></span>|<span data-ttu-id="9143b-133">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="9143b-133">UUID for the object</span></span>|
|<span data-ttu-id="9143b-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="9143b-134">eventDateTime</span></span>|<span data-ttu-id="9143b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9143b-135">DateTimeOffset</span></span>|<span data-ttu-id="9143b-136">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="9143b-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="9143b-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="9143b-137">correlationId</span></span>|<span data-ttu-id="9143b-138">String</span><span class="sxs-lookup"><span data-stu-id="9143b-138">String</span></span>|<span data-ttu-id="9143b-139">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="9143b-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="9143b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9143b-140">Response</span></span>
<span data-ttu-id="9143b-141">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9143b-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9143b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="9143b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="9143b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9143b-143">Request</span></span>
<span data-ttu-id="9143b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9143b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="9143b-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="9143b-145">Response</span></span>
<span data-ttu-id="9143b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9143b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



