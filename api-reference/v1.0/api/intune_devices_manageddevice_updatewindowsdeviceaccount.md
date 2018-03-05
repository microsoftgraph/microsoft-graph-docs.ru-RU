# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="85d0a-101">Действие updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="85d0a-101">updateWindowsDeviceAccount action</span></span>

> <span data-ttu-id="85d0a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85d0a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85d0a-103">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="85d0a-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85d0a-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85d0a-104">Prerequisites</span></span>
<span data-ttu-id="85d0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="85d0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="85d0a-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="85d0a-107">Permission type</span></span>|<span data-ttu-id="85d0a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85d0a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85d0a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85d0a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="85d0a-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="85d0a-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="85d0a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85d0a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85d0a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d0a-112">Not supported.</span></span>|
|<span data-ttu-id="85d0a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85d0a-113">Application</span></span>|<span data-ttu-id="85d0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d0a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85d0a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85d0a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="85d0a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85d0a-116">Request headers</span></span>
|<span data-ttu-id="85d0a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85d0a-117">Header</span></span>|<span data-ttu-id="85d0a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="85d0a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85d0a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d0a-119">Authorization</span></span>|<span data-ttu-id="85d0a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85d0a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85d0a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="85d0a-121">Accept</span></span>|<span data-ttu-id="85d0a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="85d0a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d0a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85d0a-123">Request body</span></span>
<span data-ttu-id="85d0a-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85d0a-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="85d0a-125">В приведенной ниже таблице показаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="85d0a-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="85d0a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="85d0a-126">Property</span></span>|<span data-ttu-id="85d0a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="85d0a-127">Type</span></span>|<span data-ttu-id="85d0a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="85d0a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85d0a-129">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="85d0a-129">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="85d0a-130">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="85d0a-130">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune_devices_updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="85d0a-131">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="85d0a-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85d0a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d0a-132">Response</span></span>
<span data-ttu-id="85d0a-133">При успешном выполнении это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="85d0a-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85d0a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="85d0a-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="85d0a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="85d0a-135">Request</span></span>
<span data-ttu-id="85d0a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85d0a-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="85d0a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="85d0a-137">Response</span></span>
<span data-ttu-id="85d0a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="85d0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



