# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="585b6-101">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="585b6-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>



> <span data-ttu-id="585b6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="585b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="585b6-103">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="585b6-103">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="585b6-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="585b6-104">Prerequisites</span></span>
<span data-ttu-id="585b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="585b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="585b6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="585b6-107">Permission type</span></span>|<span data-ttu-id="585b6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="585b6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="585b6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="585b6-109">Delegated (work or school account)</span></span>| <span data-ttu-id="585b6-110">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="585b6-110">_varies by context_</span></span> |
| <span data-ttu-id="585b6-111">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="585b6-111">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="585b6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="585b6-112">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="585b6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="585b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="585b6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585b6-114">Not supported.</span></span>|
|<span data-ttu-id="585b6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="585b6-115">Application</span></span>|<span data-ttu-id="585b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="585b6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="585b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="585b6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="585b6-118">Request headers</span></span>
|<span data-ttu-id="585b6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="585b6-119">Header</span></span>|<span data-ttu-id="585b6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="585b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="585b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="585b6-121">Authorization</span></span>|<span data-ttu-id="585b6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="585b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="585b6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="585b6-123">Accept</span></span>|<span data-ttu-id="585b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="585b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="585b6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="585b6-125">Request body</span></span>
<span data-ttu-id="585b6-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="585b6-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="585b6-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="585b6-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="585b6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="585b6-128">Property</span></span>|<span data-ttu-id="585b6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="585b6-129">Type</span></span>|<span data-ttu-id="585b6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="585b6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="585b6-131">deviceTag</span><span class="sxs-lookup"><span data-stu-id="585b6-131">deviceTag</span></span>|<span data-ttu-id="585b6-132">String</span><span class="sxs-lookup"><span data-stu-id="585b6-132">String</span></span>|<span data-ttu-id="585b6-133">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="585b6-133">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="585b6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="585b6-134">Response</span></span>
<span data-ttu-id="585b6-135">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="585b6-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="585b6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="585b6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="585b6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="585b6-137">Request</span></span>
<span data-ttu-id="585b6-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="585b6-138">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="585b6-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="585b6-139">Response</span></span>
<span data-ttu-id="585b6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="585b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



