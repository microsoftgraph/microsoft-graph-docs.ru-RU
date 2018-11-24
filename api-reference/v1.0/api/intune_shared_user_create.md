# <a name="create-user"></a><span data-ttu-id="49223-101">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="49223-101">Create user</span></span>

> <span data-ttu-id="49223-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49223-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49223-103">Создание объекта [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="49223-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49223-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49223-104">Prerequisites</span></span>
<span data-ttu-id="49223-105">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="49223-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="49223-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="49223-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="49223-107">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="49223-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="49223-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49223-108">Permission type</span></span>|<span data-ttu-id="49223-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49223-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49223-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49223-110">Delegated (work or school account)</span></span>| <span data-ttu-id="49223-111">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="49223-111">_varies by context_</span></span> |
| <span data-ttu-id="49223-112">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="49223-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="49223-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49223-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="49223-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="49223-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="49223-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49223-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="49223-116">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="49223-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="49223-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49223-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="49223-118">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="49223-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="49223-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49223-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="49223-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49223-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49223-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49223-121">Not supported.</span></span>|
|<span data-ttu-id="49223-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49223-122">Application</span></span>|<span data-ttu-id="49223-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49223-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49223-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49223-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="49223-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49223-125">Request headers</span></span>
|<span data-ttu-id="49223-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49223-126">Header</span></span>|<span data-ttu-id="49223-127">Значение</span><span class="sxs-lookup"><span data-stu-id="49223-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49223-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="49223-128">Authorization</span></span>|<span data-ttu-id="49223-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49223-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49223-130">Accept</span><span class="sxs-lookup"><span data-stu-id="49223-130">Accept</span></span>|<span data-ttu-id="49223-131">application/json</span><span class="sxs-lookup"><span data-stu-id="49223-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49223-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49223-132">Request body</span></span>
<span data-ttu-id="49223-133">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49223-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="49223-134">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="49223-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="49223-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="49223-135">Property</span></span>|<span data-ttu-id="49223-136">Тип</span><span class="sxs-lookup"><span data-stu-id="49223-136">Type</span></span>|<span data-ttu-id="49223-137">Описание</span><span class="sxs-lookup"><span data-stu-id="49223-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49223-138">id</span><span class="sxs-lookup"><span data-stu-id="49223-138">id</span></span>|<span data-ttu-id="49223-139">String</span><span class="sxs-lookup"><span data-stu-id="49223-139">String</span></span>|<span data-ttu-id="49223-140">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="49223-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="49223-141">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="49223-141">**Onboarding**</span></span>|
|<span data-ttu-id="49223-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="49223-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="49223-143">Int32</span><span class="sxs-lookup"><span data-stu-id="49223-143">Int32</span></span>|<span data-ttu-id="49223-144">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="49223-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="49223-145">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="49223-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="49223-146">Поддержка свойств текст запроса изменяется в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="49223-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="49223-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="49223-147">Response</span></span>
<span data-ttu-id="49223-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune_shared_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="49223-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49223-149">Пример</span><span class="sxs-lookup"><span data-stu-id="49223-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="49223-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="49223-150">Request</span></span>
<span data-ttu-id="49223-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49223-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="49223-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="49223-152">Response</span></span>
<span data-ttu-id="49223-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49223-153">Here is an example of the response.</span></span> <span data-ttu-id="49223-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="49223-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49223-155">Свойства, возвращенные фактический вызов различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="49223-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



