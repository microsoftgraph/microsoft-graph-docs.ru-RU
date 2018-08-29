# <a name="wipe-action"></a><span data-ttu-id="9d261-101">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="9d261-101">wipe action</span></span>

> <span data-ttu-id="9d261-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d261-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d261-103">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="9d261-103">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d261-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9d261-104">Prerequisites</span></span>
<span data-ttu-id="9d261-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d261-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d261-107">Permission type</span></span>|<span data-ttu-id="9d261-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d261-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d261-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d261-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9d261-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9d261-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9d261-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d261-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d261-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d261-112">Not supported.</span></span>|
|<span data-ttu-id="9d261-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d261-113">Application</span></span>|<span data-ttu-id="9d261-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d261-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d261-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d261-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="9d261-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d261-116">Request headers</span></span>
|<span data-ttu-id="9d261-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d261-117">Header</span></span>|<span data-ttu-id="9d261-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9d261-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d261-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d261-119">Authorization</span></span>|<span data-ttu-id="9d261-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="9d261-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d261-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9d261-121">Accept</span></span>|<span data-ttu-id="9d261-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9d261-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d261-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d261-123">Request body</span></span>
<span data-ttu-id="9d261-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d261-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9d261-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9d261-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9d261-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d261-126">Property</span></span>|<span data-ttu-id="9d261-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9d261-127">Type</span></span>|<span data-ttu-id="9d261-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9d261-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d261-129">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="9d261-129">keepEnrollmentData</span></span>|<span data-ttu-id="9d261-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d261-130">Boolean</span></span>|<span data-ttu-id="9d261-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d261-131">Not yet documented</span></span>|
|<span data-ttu-id="9d261-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="9d261-132">keepUserData</span></span>|<span data-ttu-id="9d261-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d261-133">Boolean</span></span>|<span data-ttu-id="9d261-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d261-134">Not yet documented</span></span>|
|<span data-ttu-id="9d261-135">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="9d261-135">macOsUnlockCode</span></span>|<span data-ttu-id="9d261-136">String</span><span class="sxs-lookup"><span data-stu-id="9d261-136">String</span></span>|<span data-ttu-id="9d261-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d261-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9d261-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d261-138">Response</span></span>
<span data-ttu-id="9d261-139">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9d261-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d261-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9d261-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d261-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d261-141">Request</span></span>
<span data-ttu-id="9d261-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d261-142">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe
Content-type: application/json

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="9d261-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d261-143">Response</span></span>
<span data-ttu-id="9d261-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d261-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "response" } -->
``` http
HTTP/1.1 204 No Content
```



