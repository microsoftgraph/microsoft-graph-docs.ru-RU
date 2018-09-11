# <a name="create-user"></a><span data-ttu-id="531a6-101">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="531a6-101">Create user</span></span>

> <span data-ttu-id="531a6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="531a6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="531a6-103">Создание объекта [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="531a6-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="531a6-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="531a6-104">Prerequisites</span></span>
<span data-ttu-id="531a6-105">Чтобы вызвать этот API, необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="531a6-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="531a6-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="531a6-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="531a6-107">Необходимость в каждом из разрешений зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="531a6-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="531a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="531a6-108">Permission type</span></span>|<span data-ttu-id="531a6-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="531a6-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="531a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="531a6-110">Delegated (work or school account)</span></span>| <span data-ttu-id="531a6-111">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="531a6-111">_varies by context_</span></span> |
| <span data-ttu-id="531a6-112">&nbsp; &nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="531a6-112">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="531a6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531a6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="531a6-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="531a6-114">.mam</span></span> | <span data-ttu-id="531a6-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531a6-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="531a6-116">&nbsp; &nbsp; Адаптация</span><span class="sxs-lookup"><span data-stu-id="531a6-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="531a6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531a6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="531a6-118">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="531a6-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="531a6-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="531a6-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="531a6-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="531a6-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="531a6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531a6-121">Not supported.</span></span>|
|<span data-ttu-id="531a6-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="531a6-122">Application</span></span>|<span data-ttu-id="531a6-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="531a6-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="531a6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="531a6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="531a6-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="531a6-125">Request headers</span></span>
|<span data-ttu-id="531a6-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="531a6-126">Header</span></span>|<span data-ttu-id="531a6-127">Значение</span><span class="sxs-lookup"><span data-stu-id="531a6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="531a6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="531a6-128">Authorization</span></span>|<span data-ttu-id="531a6-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="531a6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="531a6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="531a6-130">Accept</span></span>|<span data-ttu-id="531a6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="531a6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="531a6-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="531a6-132">Request body</span></span>
<span data-ttu-id="531a6-133">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="531a6-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="531a6-134">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="531a6-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="531a6-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="531a6-135">Property</span></span>|<span data-ttu-id="531a6-136">Тип</span><span class="sxs-lookup"><span data-stu-id="531a6-136">Type</span></span>|<span data-ttu-id="531a6-137">Описание</span><span class="sxs-lookup"><span data-stu-id="531a6-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="531a6-138">id</span><span class="sxs-lookup"><span data-stu-id="531a6-138">id</span></span>|<span data-ttu-id="531a6-139">String (строка)</span><span class="sxs-lookup"><span data-stu-id="531a6-139">String</span></span>|<span data-ttu-id="531a6-140">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="531a6-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="531a6-141">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="531a6-141">**On-boarding**</span></span>|
|<span data-ttu-id="531a6-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="531a6-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="531a6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="531a6-143">Int32</span></span>|<span data-ttu-id="531a6-144">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="531a6-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="531a6-145">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="531a6-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="531a6-146">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="531a6-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="531a6-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="531a6-147">Response</span></span>
<span data-ttu-id="531a6-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune_shared_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="531a6-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="531a6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="531a6-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="531a6-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="531a6-150">Request</span></span>
<span data-ttu-id="531a6-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="531a6-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="531a6-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="531a6-152">Response</span></span>
<span data-ttu-id="531a6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="531a6-153">Here is an example of the response.</span></span> <span data-ttu-id="531a6-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="531a6-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="531a6-155">Свойства, возвращенные фактическим вызовом, могут отличаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="531a6-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



