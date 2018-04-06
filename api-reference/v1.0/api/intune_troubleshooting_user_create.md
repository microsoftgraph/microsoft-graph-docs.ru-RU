# <a name="create-user"></a><span data-ttu-id="019cd-101">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="019cd-101">Create user</span></span>

> <span data-ttu-id="019cd-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="019cd-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="019cd-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019cd-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="019cd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="019cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="019cd-105">Создание объекта [user](../resources/intune_troubleshooting_user.md).</span><span class="sxs-lookup"><span data-stu-id="019cd-105">Create a new [user](../resources/intune_troubleshooting_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="019cd-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="019cd-106">Prerequisites</span></span>
<span data-ttu-id="019cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="019cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="019cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="019cd-109">Permission type</span></span>|<span data-ttu-id="019cd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="019cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="019cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="019cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="019cd-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019cd-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="019cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="019cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="019cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019cd-114">Not supported.</span></span>|
|<span data-ttu-id="019cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="019cd-115">Application</span></span>|<span data-ttu-id="019cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="019cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="019cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="019cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="019cd-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="019cd-118">Request headers</span></span>
|<span data-ttu-id="019cd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="019cd-119">Header</span></span>|<span data-ttu-id="019cd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="019cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="019cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="019cd-121">Authorization</span></span>|<span data-ttu-id="019cd-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="019cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="019cd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="019cd-123">Accept</span></span>|<span data-ttu-id="019cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="019cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="019cd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="019cd-125">Request body</span></span>
<span data-ttu-id="019cd-126">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="019cd-126">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="019cd-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="019cd-127">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="019cd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="019cd-128">Property</span></span>|<span data-ttu-id="019cd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="019cd-129">Type</span></span>|<span data-ttu-id="019cd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="019cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="019cd-131">id</span><span class="sxs-lookup"><span data-stu-id="019cd-131">id</span></span>|<span data-ttu-id="019cd-132">String</span><span class="sxs-lookup"><span data-stu-id="019cd-132">String</span></span>|<span data-ttu-id="019cd-133">Уникальный идентификатор для пользователя.</span><span class="sxs-lookup"><span data-stu-id="019cd-133">Unique Identifier for the user</span></span>|



## <a name="response"></a><span data-ttu-id="019cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="019cd-134">Response</span></span>
<span data-ttu-id="019cd-135">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune_troubleshooting_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="019cd-135">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="019cd-136">Пример</span><span class="sxs-lookup"><span data-stu-id="019cd-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="019cd-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="019cd-137">Request</span></span>
<span data-ttu-id="019cd-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="019cd-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="019cd-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="019cd-139">Response</span></span>
<span data-ttu-id="019cd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="019cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



