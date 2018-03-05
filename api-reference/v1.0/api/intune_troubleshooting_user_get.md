# <a name="get-user"></a><span data-ttu-id="27a95-101">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="27a95-101">Get user</span></span>

> <span data-ttu-id="27a95-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27a95-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27a95-103">Чтение свойств и связей объекта [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="27a95-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27a95-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="27a95-104">Prerequisites</span></span>
<span data-ttu-id="27a95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27a95-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="27a95-107">Permission type</span></span>|<span data-ttu-id="27a95-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a95-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27a95-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a95-109">Delegated (work or school account)</span></span>|<span data-ttu-id="27a95-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="27a95-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="27a95-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a95-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27a95-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a95-112">Not supported.</span></span>|
|<span data-ttu-id="27a95-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a95-113">Application</span></span>|<span data-ttu-id="27a95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a95-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27a95-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a95-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27a95-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27a95-116">Optional query parameters</span></span>
<span data-ttu-id="27a95-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="27a95-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27a95-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a95-118">Request headers</span></span>
|<span data-ttu-id="27a95-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27a95-119">Header</span></span>|<span data-ttu-id="27a95-120">Значение</span><span class="sxs-lookup"><span data-stu-id="27a95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27a95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27a95-121">Authorization</span></span>|<span data-ttu-id="27a95-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27a95-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27a95-123">Accept</span><span class="sxs-lookup"><span data-stu-id="27a95-123">Accept</span></span>|<span data-ttu-id="27a95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27a95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27a95-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27a95-125">Request body</span></span>
<span data-ttu-id="27a95-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27a95-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27a95-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a95-127">Response</span></span>
<span data-ttu-id="27a95-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune_troubleshooting_user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27a95-128">If successful, this method returns a `200 OK` response code and [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27a95-129">Пример</span><span class="sxs-lookup"><span data-stu-id="27a95-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="27a95-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a95-130">Request</span></span>
<span data-ttu-id="27a95-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a95-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="27a95-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="27a95-132">Response</span></span>
<span data-ttu-id="27a95-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="27a95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



