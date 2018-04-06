# <a name="update-devicemanagement"></a><span data-ttu-id="45d71-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="45d71-101">Update deviceManagement</span></span>

> <span data-ttu-id="45d71-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45d71-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45d71-103">Использование данных API интерфейсов в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d71-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45d71-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45d71-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45d71-105">Обновление свойств объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="45d71-105">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45d71-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45d71-106">Prerequisites</span></span>
<span data-ttu-id="45d71-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45d71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45d71-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45d71-109">Permission type</span></span>|<span data-ttu-id="45d71-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45d71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d71-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45d71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45d71-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45d71-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="45d71-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45d71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d71-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d71-114">Not supported.</span></span>|
|<span data-ttu-id="45d71-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45d71-115">Application</span></span>|<span data-ttu-id="45d71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45d71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d71-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45d71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="45d71-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45d71-118">Request headers</span></span>
|<span data-ttu-id="45d71-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45d71-119">Header</span></span>|<span data-ttu-id="45d71-120">Значение</span><span class="sxs-lookup"><span data-stu-id="45d71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d71-121">Authorization</span></span>|<span data-ttu-id="45d71-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45d71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d71-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45d71-123">Accept</span></span>|<span data-ttu-id="45d71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45d71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d71-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45d71-125">Request body</span></span>
<span data-ttu-id="45d71-126">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45d71-126">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>

<span data-ttu-id="45d71-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="45d71-127">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span></span>

|<span data-ttu-id="45d71-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="45d71-128">Property</span></span>|<span data-ttu-id="45d71-129">Тип</span><span class="sxs-lookup"><span data-stu-id="45d71-129">Type</span></span>|<span data-ttu-id="45d71-130">Описание</span><span class="sxs-lookup"><span data-stu-id="45d71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d71-131">id</span><span class="sxs-lookup"><span data-stu-id="45d71-131">id</span></span>|<span data-ttu-id="45d71-132">String</span><span class="sxs-lookup"><span data-stu-id="45d71-132">String</span></span>|<span data-ttu-id="45d71-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="45d71-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="45d71-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45d71-134">Response</span></span>
<span data-ttu-id="45d71-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45d71-135">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d71-136">Пример</span><span class="sxs-lookup"><span data-stu-id="45d71-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="45d71-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="45d71-137">Request</span></span>
<span data-ttu-id="45d71-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45d71-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="45d71-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="45d71-139">Response</span></span>
<span data-ttu-id="45d71-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45d71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



