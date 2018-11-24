# <a name="list-users"></a><span data-ttu-id="b04e0-101">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="b04e0-101">List users</span></span>

> <span data-ttu-id="b04e0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b04e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b04e0-103">Список свойств и связей объектов [user](../resources/intune_shared_user.md).</span><span class="sxs-lookup"><span data-stu-id="b04e0-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b04e0-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b04e0-104">Prerequisites</span></span>
<span data-ttu-id="b04e0-105">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="b04e0-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b04e0-106">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b04e0-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="b04e0-107">Конкретные разрешения зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="b04e0-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="b04e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b04e0-108">Permission type</span></span>|<span data-ttu-id="b04e0-109">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b04e0-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b04e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b04e0-110">Delegated (work or school account)</span></span>| <span data-ttu-id="b04e0-111">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="b04e0-111">_varies by context_</span></span>|
| <span data-ttu-id="b04e0-112">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="b04e0-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="b04e0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04e0-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b04e0-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="b04e0-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="b04e0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04e0-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b04e0-116">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="b04e0-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="b04e0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04e0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b04e0-118">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="b04e0-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b04e0-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b04e0-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="b04e0-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b04e0-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b04e0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04e0-121">Not supported.</span></span>|
|<span data-ttu-id="b04e0-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b04e0-122">Application</span></span>|<span data-ttu-id="b04e0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04e0-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b04e0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b04e0-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="b04e0-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b04e0-125">Request headers</span></span>
|<span data-ttu-id="b04e0-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b04e0-126">Header</span></span>|<span data-ttu-id="b04e0-127">Значение</span><span class="sxs-lookup"><span data-stu-id="b04e0-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b04e0-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b04e0-128">Authorization</span></span>|<span data-ttu-id="b04e0-129">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b04e0-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b04e0-130">Accept</span><span class="sxs-lookup"><span data-stu-id="b04e0-130">Accept</span></span>|<span data-ttu-id="b04e0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b04e0-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b04e0-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b04e0-132">Request body</span></span>
<span data-ttu-id="b04e0-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b04e0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b04e0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b04e0-134">Response</span></span>
<span data-ttu-id="b04e0-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune_shared_user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b04e0-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b04e0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b04e0-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b04e0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b04e0-137">Request</span></span>
<span data-ttu-id="b04e0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b04e0-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="b04e0-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b04e0-139">Response</span></span>
<span data-ttu-id="b04e0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b04e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



