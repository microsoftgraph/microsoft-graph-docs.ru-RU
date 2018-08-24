# <a name="delete-user"></a><span data-ttu-id="63adf-101">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="63adf-101">Delete user</span></span>

> <span data-ttu-id="63adf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="63adf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63adf-103">Удаляет объект [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="63adf-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63adf-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63adf-104">Prerequisites</span></span>
<span data-ttu-id="63adf-105">Чтобы вызвать этот API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="63adf-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="63adf-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63adf-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="63adf-107">Конкретное обязательное   разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="63adf-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="63adf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63adf-108">Permission type</span></span>|<span data-ttu-id="63adf-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63adf-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63adf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63adf-110">Delegated (work or school account)</span></span>| <span data-ttu-id="63adf-111">_Изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="63adf-111">_varies by context_</span></span>|
| <span data-ttu-id="63adf-112">&nbsp; &nbsp; Устройства</span><span class="sxs-lookup"><span data-stu-id="63adf-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="63adf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63adf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="63adf-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="63adf-114">.mam</span></span> | <span data-ttu-id="63adf-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63adf-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="63adf-116">&nbsp; &nbsp; Адаптация</span><span class="sxs-lookup"><span data-stu-id="63adf-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="63adf-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63adf-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63adf-118">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="63adf-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="63adf-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63adf-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="63adf-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63adf-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63adf-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63adf-121">Not supported.</span></span>|
|<span data-ttu-id="63adf-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63adf-122">Application</span></span>|<span data-ttu-id="63adf-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63adf-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63adf-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63adf-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="63adf-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63adf-125">Request headers</span></span>
|<span data-ttu-id="63adf-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63adf-126">Header</span></span>|<span data-ttu-id="63adf-127">Значение</span><span class="sxs-lookup"><span data-stu-id="63adf-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63adf-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63adf-128">Authorization</span></span>|<span data-ttu-id="63adf-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63adf-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63adf-130">Accept</span><span class="sxs-lookup"><span data-stu-id="63adf-130">Accept</span></span>|<span data-ttu-id="63adf-131">application/json</span><span class="sxs-lookup"><span data-stu-id="63adf-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63adf-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63adf-132">Request body</span></span>
<span data-ttu-id="63adf-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63adf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63adf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="63adf-134">Response</span></span>
<span data-ttu-id="63adf-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63adf-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63adf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="63adf-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="63adf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="63adf-137">Request</span></span>
<span data-ttu-id="63adf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63adf-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="63adf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="63adf-139">Response</span></span>
<span data-ttu-id="63adf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="63adf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



