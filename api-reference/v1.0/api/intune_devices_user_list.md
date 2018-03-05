# <a name="list-users"></a><span data-ttu-id="1d86a-101">List users</span><span class="sxs-lookup"><span data-stu-id="1d86a-101">List users</span></span>

> <span data-ttu-id="1d86a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d86a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d86a-103">Перечисление свойств и связей объектов [user](../resources/intune_devices_user.md).</span><span class="sxs-lookup"><span data-stu-id="1d86a-103">List properties and relationships of the [user](../resources/intune_devices_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d86a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1d86a-104">Prerequisites</span></span>
<span data-ttu-id="1d86a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d86a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d86a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d86a-107">Permission type</span></span>|<span data-ttu-id="1d86a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d86a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d86a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d86a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1d86a-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d86a-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1d86a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d86a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d86a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d86a-112">Not supported.</span></span>|
|<span data-ttu-id="1d86a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d86a-113">Application</span></span>|<span data-ttu-id="1d86a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d86a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d86a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d86a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="1d86a-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1d86a-116">Request headers</span></span>
|<span data-ttu-id="1d86a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d86a-117">Header</span></span>|<span data-ttu-id="1d86a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1d86a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d86a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d86a-119">Authorization</span></span>|<span data-ttu-id="1d86a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d86a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d86a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1d86a-121">Accept</span></span>|<span data-ttu-id="1d86a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1d86a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d86a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d86a-123">Request body</span></span>
<span data-ttu-id="1d86a-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d86a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d86a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d86a-125">Response</span></span>
<span data-ttu-id="1d86a-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [user](../resources/intune_devices_user.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d86a-126">If successful, this method returns a `200 OK` response code and collection of [user](../resources/intune_devices_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d86a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1d86a-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d86a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d86a-128">Request</span></span>
<span data-ttu-id="1d86a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d86a-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="1d86a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d86a-130">Response</span></span>
<span data-ttu-id="1d86a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d86a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



