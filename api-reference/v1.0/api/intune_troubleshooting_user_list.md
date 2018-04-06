# <a name="list-users"></a><span data-ttu-id="2ada6-101">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="2ada6-101">List users</span></span>

> <span data-ttu-id="2ada6-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ada6-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ada6-103">Использование данных API интерфейсов в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ada6-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ada6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ada6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ada6-105">Список свойств и связей объектов [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="2ada6-105">List properties and relationships of the [user](../resources/intune_troubleshooting_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ada6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ada6-106">Prerequisites</span></span>
<span data-ttu-id="2ada6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ada6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ada6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ada6-109">Permission type</span></span>|<span data-ttu-id="2ada6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ada6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ada6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ada6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ada6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ada6-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2ada6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ada6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ada6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ada6-114">Not supported.</span></span>|
|<span data-ttu-id="2ada6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ada6-115">Application</span></span>|<span data-ttu-id="2ada6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ada6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ada6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ada6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="2ada6-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ada6-118">Request headers</span></span>
|<span data-ttu-id="2ada6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ada6-119">Header</span></span>|<span data-ttu-id="2ada6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2ada6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ada6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ada6-121">Authorization</span></span>|<span data-ttu-id="2ada6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ada6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ada6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2ada6-123">Accept</span></span>|<span data-ttu-id="2ada6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2ada6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ada6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ada6-125">Request body</span></span>
<span data-ttu-id="2ada6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ada6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ada6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ada6-127">Response</span></span>
<span data-ttu-id="2ada6-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune_troubleshooting_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ada6-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_troubleshooting_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ada6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2ada6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ada6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ada6-130">Request</span></span>
<span data-ttu-id="2ada6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ada6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="2ada6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ada6-132">Response</span></span>
<span data-ttu-id="2ada6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2ada6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



