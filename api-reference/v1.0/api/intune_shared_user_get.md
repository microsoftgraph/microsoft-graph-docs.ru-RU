# <a name="get-user"></a><span data-ttu-id="e1b07-101">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="e1b07-101">Get user</span></span>

> <span data-ttu-id="e1b07-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1b07-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1b07-103">Чтение свойств и связей объекта [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="e1b07-103">Read properties and relationships of the [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1b07-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1b07-104">Prerequisites</span></span>
<span data-ttu-id="e1b07-105">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="e1b07-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e1b07-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1b07-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="e1b07-107">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="e1b07-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="e1b07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b07-108">Permission type</span></span>|<span data-ttu-id="e1b07-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1b07-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1b07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1b07-110">Delegated (work or school account)</span></span>| <span data-ttu-id="e1b07-111">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="e1b07-111">_varies by context_</span></span>|
| <span data-ttu-id="e1b07-112">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="e1b07-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="e1b07-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b07-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e1b07-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e1b07-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e1b07-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b07-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e1b07-116">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="e1b07-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="e1b07-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b07-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e1b07-118">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e1b07-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e1b07-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1b07-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="e1b07-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1b07-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1b07-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b07-121">Not supported.</span></span>|
|<span data-ttu-id="e1b07-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1b07-122">Application</span></span>|<span data-ttu-id="e1b07-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b07-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1b07-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1b07-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1b07-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1b07-125">Optional query parameters</span></span>
<span data-ttu-id="e1b07-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1b07-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e1b07-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1b07-127">Request headers</span></span>
|<span data-ttu-id="e1b07-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1b07-128">Header</span></span>|<span data-ttu-id="e1b07-129">Значение</span><span class="sxs-lookup"><span data-stu-id="e1b07-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1b07-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1b07-130">Authorization</span></span>|<span data-ttu-id="e1b07-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e1b07-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1b07-132">Accept</span><span class="sxs-lookup"><span data-stu-id="e1b07-132">Accept</span></span>|<span data-ttu-id="e1b07-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b07-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1b07-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1b07-134">Request body</span></span>
<span data-ttu-id="e1b07-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1b07-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b07-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1b07-136">Response</span></span>
<span data-ttu-id="e1b07-137">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune_shared_user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1b07-137">If successful, this method returns a `200 OK` response code and [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b07-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e1b07-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1b07-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1b07-139">Request</span></span>
<span data-ttu-id="e1b07-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1b07-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="e1b07-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1b07-141">Response</span></span>
<span data-ttu-id="e1b07-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e1b07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



