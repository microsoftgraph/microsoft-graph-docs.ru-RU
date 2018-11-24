# <a name="delete-user"></a><span data-ttu-id="b6018-101">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="b6018-101">Delete user</span></span>

> <span data-ttu-id="b6018-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6018-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6018-103">Удаляет объект [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="b6018-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6018-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6018-104">Prerequisites</span></span>
<span data-ttu-id="b6018-105">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b6018-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6018-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b6018-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="b6018-107">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="b6018-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="b6018-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6018-108">Permission type</span></span>|<span data-ttu-id="b6018-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6018-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6018-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6018-110">Delegated (work or school account)</span></span>| <span data-ttu-id="b6018-111">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="b6018-111">_varies by context_</span></span>|
| <span data-ttu-id="b6018-112">&nbsp;&nbsp; Устройств</span><span class="sxs-lookup"><span data-stu-id="b6018-112">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="b6018-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6018-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="b6018-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b6018-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="b6018-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6018-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="b6018-116">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="b6018-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="b6018-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6018-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="b6018-118">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b6018-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b6018-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6018-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="b6018-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6018-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6018-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6018-121">Not supported.</span></span>|
|<span data-ttu-id="b6018-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6018-122">Application</span></span>|<span data-ttu-id="b6018-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6018-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6018-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6018-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="b6018-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6018-125">Request headers</span></span>
|<span data-ttu-id="b6018-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6018-126">Header</span></span>|<span data-ttu-id="b6018-127">Значение</span><span class="sxs-lookup"><span data-stu-id="b6018-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6018-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6018-128">Authorization</span></span>|<span data-ttu-id="b6018-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b6018-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6018-130">Accept</span><span class="sxs-lookup"><span data-stu-id="b6018-130">Accept</span></span>|<span data-ttu-id="b6018-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b6018-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6018-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6018-132">Request body</span></span>
<span data-ttu-id="b6018-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6018-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6018-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6018-134">Response</span></span>
<span data-ttu-id="b6018-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6018-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6018-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b6018-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6018-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6018-137">Request</span></span>
<span data-ttu-id="b6018-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6018-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="b6018-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6018-139">Response</span></span>
<span data-ttu-id="b6018-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b6018-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



