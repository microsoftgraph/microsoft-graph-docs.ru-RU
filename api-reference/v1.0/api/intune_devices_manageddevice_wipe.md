# <a name="wipe-action"></a><span data-ttu-id="1fc48-101">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="1fc48-101">wipe action</span></span>

> <span data-ttu-id="1fc48-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1fc48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fc48-103">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="1fc48-103">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fc48-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1fc48-104">Prerequisites</span></span>
<span data-ttu-id="1fc48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1fc48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1fc48-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fc48-107">Permission type</span></span>|<span data-ttu-id="1fc48-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fc48-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fc48-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fc48-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1fc48-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1fc48-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1fc48-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fc48-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fc48-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fc48-112">Not supported.</span></span>|
|<span data-ttu-id="1fc48-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fc48-113">Application</span></span>|<span data-ttu-id="1fc48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fc48-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fc48-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fc48-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="1fc48-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fc48-116">Request headers</span></span>
|<span data-ttu-id="1fc48-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fc48-117">Header</span></span>|<span data-ttu-id="1fc48-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1fc48-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fc48-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fc48-119">Authorization</span></span>|<span data-ttu-id="1fc48-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fc48-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fc48-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1fc48-121">Accept</span></span>|<span data-ttu-id="1fc48-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1fc48-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc48-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fc48-123">Request body</span></span>
<span data-ttu-id="1fc48-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fc48-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1fc48-125">В следующей таблице показаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="1fc48-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1fc48-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fc48-126">Property</span></span>|<span data-ttu-id="1fc48-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1fc48-127">Type</span></span>|<span data-ttu-id="1fc48-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1fc48-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fc48-129">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="1fc48-129">keepEnrollmentData</span></span>|<span data-ttu-id="1fc48-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fc48-130">Boolean</span></span>|<span data-ttu-id="1fc48-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1fc48-131">Not yet documented</span></span>|
|<span data-ttu-id="1fc48-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="1fc48-132">keepUserData</span></span>|<span data-ttu-id="1fc48-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fc48-133">Boolean</span></span>|<span data-ttu-id="1fc48-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1fc48-134">Not yet documented</span></span>|
|<span data-ttu-id="1fc48-135">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="1fc48-135">macOsUnlockCode</span></span>|<span data-ttu-id="1fc48-136">String</span><span class="sxs-lookup"><span data-stu-id="1fc48-136">String</span></span>|<span data-ttu-id="1fc48-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1fc48-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1fc48-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fc48-138">Response</span></span>
<span data-ttu-id="1fc48-139">В случае успешного выполнения этот метод возвращает код ответа `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1fc48-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1fc48-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1fc48-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fc48-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc48-141">Request</span></span>
<span data-ttu-id="1fc48-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fc48-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="1fc48-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fc48-143">Response</span></span>
<span data-ttu-id="1fc48-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1fc48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



