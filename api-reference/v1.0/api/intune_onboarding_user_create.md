# <a name="create-user"></a><span data-ttu-id="a8a9f-101">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="a8a9f-101">Create User</span></span>

> <span data-ttu-id="a8a9f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8a9f-103">Создание объекта [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="a8a9f-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8a9f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a8a9f-104">Prerequisites</span></span>
<span data-ttu-id="a8a9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a8a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8a9f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8a9f-107">Permission type</span></span>|<span data-ttu-id="a8a9f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8a9f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8a9f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8a9f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a8a9f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a9f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a8a9f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8a9f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a9f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-112">Not supported.</span></span>|
|<span data-ttu-id="a8a9f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8a9f-113">Application</span></span>|<span data-ttu-id="a8a9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8a9f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8a9f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="a8a9f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8a9f-116">Request headers</span></span>
|<span data-ttu-id="a8a9f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8a9f-117">Header</span></span>|<span data-ttu-id="a8a9f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a8a9f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8a9f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8a9f-119">Authorization</span></span>|<span data-ttu-id="a8a9f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8a9f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a8a9f-121">Accept</span></span>|<span data-ttu-id="a8a9f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a8a9f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a9f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8a9f-123">Request body</span></span>
<span data-ttu-id="a8a9f-124">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="a8a9f-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a8a9f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8a9f-126">Property</span></span>|<span data-ttu-id="a8a9f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a8a9f-127">Type</span></span>|<span data-ttu-id="a8a9f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a8a9f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a9f-129">id</span><span class="sxs-lookup"><span data-stu-id="a8a9f-129">id</span></span>|<span data-ttu-id="a8a9f-130">String</span><span class="sxs-lookup"><span data-stu-id="a8a9f-130">String</span></span>|<span data-ttu-id="a8a9f-131">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="a8a9f-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="a8a9f-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="a8a9f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a8a9f-133">Int32</span></span>|<span data-ttu-id="a8a9f-134">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="a8a9f-135">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="a8a9f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8a9f-136">Response</span></span>
<span data-ttu-id="a8a9f-137">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune_onboarding_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-137">If successful, this method returns a `201 Created` response code and [user](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a9f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a8a9f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8a9f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8a9f-139">Request</span></span>
<span data-ttu-id="a8a9f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="a8a9f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8a9f-141">Response</span></span>
<span data-ttu-id="a8a9f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8a9f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



