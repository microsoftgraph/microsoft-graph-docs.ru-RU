# <a name="update-user"></a><span data-ttu-id="a64ee-101">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="a64ee-101">Update user</span></span>

> <span data-ttu-id="a64ee-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a64ee-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a64ee-103">Использование этих API в рабочих приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a64ee-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a64ee-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a64ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a64ee-105">Обновление свойств объекта [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="a64ee-105">Update the properties of a [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a64ee-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a64ee-106">Prerequisites</span></span>
<span data-ttu-id="a64ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a64ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a64ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a64ee-109">Permission type</span></span>|<span data-ttu-id="a64ee-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a64ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a64ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a64ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a64ee-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a64ee-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a64ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a64ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a64ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a64ee-114">Not supported.</span></span>|
|<span data-ttu-id="a64ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a64ee-115">Application</span></span>|<span data-ttu-id="a64ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a64ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a64ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a64ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="a64ee-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a64ee-118">Request headers</span></span>
|<span data-ttu-id="a64ee-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a64ee-119">Header</span></span>|<span data-ttu-id="a64ee-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a64ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a64ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a64ee-121">Authorization</span></span>|<span data-ttu-id="a64ee-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a64ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a64ee-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a64ee-123">Accept</span></span>|<span data-ttu-id="a64ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a64ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a64ee-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a64ee-125">Request body</span></span>
<span data-ttu-id="a64ee-126">В теле запроса добавьте представление объекта [user](../resources/intune_troubleshooting_user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a64ee-126">In the request body, supply a JSON representation for the [user](../resources/intune_troubleshooting_user.md) object.</span></span>

<span data-ttu-id="a64ee-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="a64ee-127">The following table shows the properties that are required when you create the [user](../resources/intune_troubleshooting_user.md).</span></span>

|<span data-ttu-id="a64ee-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a64ee-128">Property</span></span>|<span data-ttu-id="a64ee-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a64ee-129">Type</span></span>|<span data-ttu-id="a64ee-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a64ee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a64ee-131">id</span><span class="sxs-lookup"><span data-stu-id="a64ee-131">id</span></span>|<span data-ttu-id="a64ee-132">String</span><span class="sxs-lookup"><span data-stu-id="a64ee-132">String</span></span>|<span data-ttu-id="a64ee-133">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a64ee-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="a64ee-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a64ee-134">Response</span></span>
<span data-ttu-id="a64ee-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune_troubleshooting_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a64ee-135">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a64ee-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a64ee-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="a64ee-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a64ee-137">Request</span></span>
<span data-ttu-id="a64ee-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a64ee-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="a64ee-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a64ee-139">Response</span></span>
<span data-ttu-id="a64ee-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a64ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



