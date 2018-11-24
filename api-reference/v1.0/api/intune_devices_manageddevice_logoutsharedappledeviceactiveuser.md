# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="efe7c-101">Действие logoutSharedAppleDeviceActiveUser</span><span class="sxs-lookup"><span data-stu-id="efe7c-101">logoutSharedAppleDeviceActiveUser action</span></span>

> <span data-ttu-id="efe7c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="efe7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efe7c-103">Выход от имени активного пользователя общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="efe7c-103">Logout shared Apple device active user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efe7c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="efe7c-104">Prerequisites</span></span>
<span data-ttu-id="efe7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="efe7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="efe7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efe7c-107">Permission type</span></span>|<span data-ttu-id="efe7c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efe7c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efe7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efe7c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="efe7c-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="efe7c-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="efe7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efe7c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe7c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efe7c-112">Not supported.</span></span>|
|<span data-ttu-id="efe7c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efe7c-113">Application</span></span>|<span data-ttu-id="efe7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efe7c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efe7c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="efe7c-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efe7c-116">Request headers</span></span>
|<span data-ttu-id="efe7c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efe7c-117">Header</span></span>|<span data-ttu-id="efe7c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="efe7c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efe7c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="efe7c-119">Authorization</span></span>|<span data-ttu-id="efe7c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efe7c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efe7c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="efe7c-121">Accept</span></span>|<span data-ttu-id="efe7c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="efe7c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe7c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efe7c-123">Request body</span></span>
<span data-ttu-id="efe7c-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efe7c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efe7c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="efe7c-125">Response</span></span>
<span data-ttu-id="efe7c-126">В случае успешного выполнения этот метод возвращает код ответа `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="efe7c-126">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="efe7c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="efe7c-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="efe7c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="efe7c-128">Request</span></span>
<span data-ttu-id="efe7c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efe7c-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="efe7c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="efe7c-130">Response</span></span>
<span data-ttu-id="efe7c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="efe7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



