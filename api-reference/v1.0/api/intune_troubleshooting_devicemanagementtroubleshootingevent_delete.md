# <a name="delete-devicemanagementtroubleshootingevent"></a><span data-ttu-id="8c758-101">Удаление объекта deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8c758-101">Delete deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="8c758-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c758-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c758-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c758-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c758-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c758-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c758-105">Удаляет объект [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="8c758-105">Deletes a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c758-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c758-106">Prerequisites</span></span>
<span data-ttu-id="8c758-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c758-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c758-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c758-109">Permission type</span></span>|<span data-ttu-id="8c758-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c758-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c758-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c758-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c758-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c758-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8c758-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c758-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c758-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c758-114">Not supported.</span></span>|
|<span data-ttu-id="8c758-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c758-115">Application</span></span>|<span data-ttu-id="8c758-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c758-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c758-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c758-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="8c758-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c758-118">Request headers</span></span>
|<span data-ttu-id="8c758-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c758-119">Header</span></span>|<span data-ttu-id="8c758-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8c758-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c758-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c758-121">Authorization</span></span>|<span data-ttu-id="8c758-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c758-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c758-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8c758-123">Accept</span></span>|<span data-ttu-id="8c758-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c758-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c758-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c758-125">Request body</span></span>
<span data-ttu-id="8c758-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c758-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c758-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c758-127">Response</span></span>
<span data-ttu-id="8c758-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8c758-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c758-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8c758-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c758-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c758-130">Request</span></span>
<span data-ttu-id="8c758-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c758-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="8c758-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c758-132">Response</span></span>
<span data-ttu-id="8c758-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8c758-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



