# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="b9dba-101">Действие deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="b9dba-101">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="b9dba-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9dba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9dba-103">Удаление пользователя на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="b9dba-103">Delete user from shared Apple device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9dba-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b9dba-104">Prerequisites</span></span>
<span data-ttu-id="b9dba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9dba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9dba-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="b9dba-107">Permission type</span></span>|<span data-ttu-id="b9dba-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9dba-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9dba-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9dba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b9dba-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b9dba-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b9dba-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9dba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9dba-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9dba-112">Not supported.</span></span>|
|<span data-ttu-id="b9dba-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9dba-113">Application</span></span>|<span data-ttu-id="b9dba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9dba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9dba-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9dba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="b9dba-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9dba-116">Request headers</span></span>
|<span data-ttu-id="b9dba-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9dba-117">Header</span></span>|<span data-ttu-id="b9dba-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b9dba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9dba-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9dba-119">Authorization</span></span>|<span data-ttu-id="b9dba-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9dba-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9dba-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b9dba-121">Accept</span></span>|<span data-ttu-id="b9dba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b9dba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9dba-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9dba-123">Request body</span></span>
<span data-ttu-id="b9dba-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9dba-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b9dba-125">В приведенной ниже таблице показаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b9dba-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b9dba-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9dba-126">Property</span></span>|<span data-ttu-id="b9dba-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b9dba-127">Type</span></span>|<span data-ttu-id="b9dba-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b9dba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9dba-129">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9dba-129">userPrincipalName</span></span>|<span data-ttu-id="b9dba-130">String</span><span class="sxs-lookup"><span data-stu-id="b9dba-130">String</span></span>|<span data-ttu-id="b9dba-131">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="b9dba-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9dba-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9dba-132">Response</span></span>
<span data-ttu-id="b9dba-133">При успешном выполнении это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9dba-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9dba-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b9dba-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9dba-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9dba-135">Request</span></span>
<span data-ttu-id="b9dba-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9dba-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b9dba-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9dba-137">Response</span></span>
<span data-ttu-id="b9dba-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9dba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



