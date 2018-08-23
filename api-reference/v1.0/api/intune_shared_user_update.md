# <a name="update-user"></a><span data-ttu-id="b49d0-101">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="b49d0-101">Update user</span></span>

> <span data-ttu-id="b49d0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b49d0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b49d0-103">Обновление свойств объекта [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="b49d0-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b49d0-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b49d0-104">Prerequisites</span></span>
<span data-ttu-id="b49d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b49d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b49d0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b49d0-107">Permission type</span></span>|<span data-ttu-id="b49d0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b49d0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b49d0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b49d0-109">Delegated (work or school account)</span></span>| <span data-ttu-id="b49d0-110">_изменяется в соответствии с контекстом_</span><span class="sxs-lookup"><span data-stu-id="b49d0-110">_varies by context_</span></span>|
| <span data-ttu-id="b49d0-111">&nbsp; &nbsp; Устройства</span><span class="sxs-lookup"><span data-stu-id="b49d0-111">&nbsp;&nbsp;</span></span> | <span data-ttu-id="b49d0-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49d0-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b49d0-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b49d0-113">.mam</span></span> | <span data-ttu-id="b49d0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49d0-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b49d0-115">&nbsp; &nbsp; Адаптация</span><span class="sxs-lookup"><span data-stu-id="b49d0-115">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="b49d0-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49d0-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="b49d0-117">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b49d0-117">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="b49d0-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b49d0-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="b49d0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b49d0-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b49d0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b49d0-120">Not supported.</span></span>|
|<span data-ttu-id="b49d0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b49d0-121">Application</span></span>|<span data-ttu-id="b49d0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b49d0-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b49d0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b49d0-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="b49d0-124">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b49d0-124">Request headers</span></span>
|<span data-ttu-id="b49d0-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b49d0-125">Header</span></span>|<span data-ttu-id="b49d0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b49d0-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b49d0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b49d0-127">Authorization</span></span>|<span data-ttu-id="b49d0-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b49d0-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b49d0-129">Accept</span><span class="sxs-lookup"><span data-stu-id="b49d0-129">Accept</span></span>|<span data-ttu-id="b49d0-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b49d0-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b49d0-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b49d0-131">Request body</span></span>
<span data-ttu-id="b49d0-132">В теле запроса добавьте представление объекта [user](../resources/intune_shared_user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b49d0-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="b49d0-133">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="b49d0-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="b49d0-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b49d0-134">Property</span></span>|<span data-ttu-id="b49d0-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b49d0-135">Type</span></span>|<span data-ttu-id="b49d0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b49d0-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b49d0-137">id</span><span class="sxs-lookup"><span data-stu-id="b49d0-137">id</span></span>|<span data-ttu-id="b49d0-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b49d0-138">String</span></span>|<span data-ttu-id="b49d0-139">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="b49d0-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="b49d0-140">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="b49d0-140">**On-boarding**</span></span>|
|<span data-ttu-id="b49d0-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="b49d0-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="b49d0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b49d0-142">Int32</span></span>|<span data-ttu-id="b49d0-143">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="b49d0-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="b49d0-144">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="b49d0-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="b49d0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b49d0-145">Response</span></span>
<span data-ttu-id="b49d0-146">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune_shared_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b49d0-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b49d0-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b49d0-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b49d0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b49d0-148">Request</span></span>
<span data-ttu-id="b49d0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b49d0-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b49d0-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="b49d0-150">Response</span></span>
<span data-ttu-id="b49d0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b49d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



