# <a name="update-user"></a><span data-ttu-id="29145-101">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="29145-101">Update user</span></span>

> <span data-ttu-id="29145-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29145-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29145-103">Обновление свойств объекта [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="29145-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29145-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="29145-104">Prerequisites</span></span>
<span data-ttu-id="29145-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29145-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29145-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29145-107">Permission type</span></span>|<span data-ttu-id="29145-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="29145-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29145-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29145-109">Delegated (work or school account)</span></span>|<span data-ttu-id="29145-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29145-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29145-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29145-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29145-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29145-112">Not supported.</span></span>|
|<span data-ttu-id="29145-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29145-113">Application</span></span>|<span data-ttu-id="29145-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29145-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29145-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29145-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="29145-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29145-116">Request headers</span></span>
|<span data-ttu-id="29145-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="29145-117">Header</span></span>|<span data-ttu-id="29145-118">Значение</span><span class="sxs-lookup"><span data-stu-id="29145-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29145-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="29145-119">Authorization</span></span>|<span data-ttu-id="29145-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29145-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29145-121">Accept</span><span class="sxs-lookup"><span data-stu-id="29145-121">Accept</span></span>|<span data-ttu-id="29145-122">application/json</span><span class="sxs-lookup"><span data-stu-id="29145-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29145-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29145-123">Request body</span></span>
<span data-ttu-id="29145-124">В теле запроса добавьте представление объекта [user](../resources/intune_onboarding_user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29145-124">In the request body, supply a JSON representation of [user](../resources/intune_onboarding_user.md) object.</span></span>

<span data-ttu-id="29145-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune_onboarding_user.md).</span><span class="sxs-lookup"><span data-stu-id="29145-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="29145-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="29145-126">Property</span></span>|<span data-ttu-id="29145-127">Тип</span><span class="sxs-lookup"><span data-stu-id="29145-127">Type</span></span>|<span data-ttu-id="29145-128">Описание</span><span class="sxs-lookup"><span data-stu-id="29145-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29145-129">id</span><span class="sxs-lookup"><span data-stu-id="29145-129">id</span></span>|<span data-ttu-id="29145-130">String</span><span class="sxs-lookup"><span data-stu-id="29145-130">String</span></span>|<span data-ttu-id="29145-131">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="29145-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="29145-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="29145-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="29145-133">Int32</span><span class="sxs-lookup"><span data-stu-id="29145-133">Int32</span></span>|<span data-ttu-id="29145-134">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="29145-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="29145-135">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="29145-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="29145-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="29145-136">Response</span></span>
<span data-ttu-id="29145-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune_onboarding_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="29145-137">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29145-138">Пример</span><span class="sxs-lookup"><span data-stu-id="29145-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="29145-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="29145-139">Request</span></span>
<span data-ttu-id="29145-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29145-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 34

{
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="29145-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="29145-141">Response</span></span>
<span data-ttu-id="29145-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="29145-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



