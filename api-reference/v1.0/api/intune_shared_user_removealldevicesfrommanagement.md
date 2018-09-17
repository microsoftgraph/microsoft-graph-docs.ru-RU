# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="64faf-101">Действие removeAllDevicesFromManagement</span><span class="sxs-lookup"><span data-stu-id="64faf-101">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="64faf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64faf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64faf-103">Прекращение управления всеми устройствами для этого пользователя</span><span class="sxs-lookup"><span data-stu-id="64faf-103">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64faf-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64faf-104">Prerequisites</span></span>
<span data-ttu-id="64faf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64faf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64faf-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64faf-107">Permission type</span></span>|<span data-ttu-id="64faf-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64faf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64faf-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64faf-109">Delegated (work or school account)</span></span>| <span data-ttu-id="64faf-110">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="64faf-110">_varies by context_</span></span> |
| <span data-ttu-id="64faf-111">&nbsp; &nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="64faf-111">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="64faf-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="64faf-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="64faf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64faf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64faf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64faf-114">Not supported.</span></span>|
|<span data-ttu-id="64faf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64faf-115">Application</span></span>|<span data-ttu-id="64faf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64faf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64faf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64faf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="64faf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64faf-118">Request headers</span></span>
|<span data-ttu-id="64faf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64faf-119">Header</span></span>|<span data-ttu-id="64faf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="64faf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64faf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64faf-121">Authorization</span></span>|<span data-ttu-id="64faf-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="64faf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64faf-123">Принять</span><span class="sxs-lookup"><span data-stu-id="64faf-123">Accept</span></span>|<span data-ttu-id="64faf-124">приложение/json</span><span class="sxs-lookup"><span data-stu-id="64faf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64faf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64faf-125">Request body</span></span>
<span data-ttu-id="64faf-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64faf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64faf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="64faf-127">Response</span></span>
<span data-ttu-id="64faf-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="64faf-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="64faf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="64faf-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="64faf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="64faf-130">Request</span></span>
<span data-ttu-id="64faf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64faf-131">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="64faf-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="64faf-132">Response</span></span>
<span data-ttu-id="64faf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64faf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



