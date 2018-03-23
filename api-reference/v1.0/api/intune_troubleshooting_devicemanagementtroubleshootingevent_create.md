# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="7fb84-101">Создание объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="7fb84-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="7fb84-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7fb84-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fb84-103">Создание объекта [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fb84-103">Create a new [plannerBucket](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fb84-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7fb84-104">Prerequisites</span></span>
<span data-ttu-id="7fb84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fb84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7fb84-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb84-107">Permission type</span></span>|<span data-ttu-id="7fb84-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fb84-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb84-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fb84-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb84-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb84-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7fb84-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fb84-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb84-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb84-112">Not supported.</span></span>|
|<span data-ttu-id="7fb84-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fb84-113">Application</span></span>|<span data-ttu-id="7fb84-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb84-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb84-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fb84-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="7fb84-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fb84-116">Request headers</span></span>
|<span data-ttu-id="7fb84-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fb84-117">Header</span></span>|<span data-ttu-id="7fb84-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7fb84-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb84-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fb84-119">Authorization</span></span>|<span data-ttu-id="7fb84-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fb84-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7fb84-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7fb84-121">Accept</span></span>|<span data-ttu-id="7fb84-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb84-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb84-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fb84-123">Request body</span></span>
<span data-ttu-id="7fb84-124">В теле запроса добавьте представление объекта deviceManagementTroubleshootingEvent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fb84-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="7fb84-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementTroubleshootingEvent.</span><span class="sxs-lookup"><span data-stu-id="7fb84-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7fb84-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fb84-126">Property</span></span>|<span data-ttu-id="7fb84-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7fb84-127">Type</span></span>|<span data-ttu-id="7fb84-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7fb84-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb84-129">id</span><span class="sxs-lookup"><span data-stu-id="7fb84-129">id</span></span>|<span data-ttu-id="7fb84-130">String</span><span class="sxs-lookup"><span data-stu-id="7fb84-130">String</span></span>|<span data-ttu-id="7fb84-131">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="7fb84-131">UUID for the object</span></span>|
|<span data-ttu-id="7fb84-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="7fb84-132">eventDateTime</span></span>|<span data-ttu-id="7fb84-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fb84-133">DateTimeOffset</span></span>|<span data-ttu-id="7fb84-134">Время возникновения события.</span><span class="sxs-lookup"><span data-stu-id="7fb84-134">Time when the event occurred .</span></span>|
|<span data-ttu-id="7fb84-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="7fb84-135">correlationId</span></span>|<span data-ttu-id="7fb84-136">String</span><span class="sxs-lookup"><span data-stu-id="7fb84-136">String</span></span>|<span data-ttu-id="7fb84-137">Идентификатор, используемый для трассировки сбоя в службе.</span><span class="sxs-lookup"><span data-stu-id="7fb84-137">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="7fb84-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fb84-138">Response</span></span>
<span data-ttu-id="7fb84-139">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7fb84-139">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb84-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7fb84-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fb84-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fb84-141">Request</span></span>
<span data-ttu-id="7fb84-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb84-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="7fb84-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb84-143">Response</span></span>
<span data-ttu-id="7fb84-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7fb84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



