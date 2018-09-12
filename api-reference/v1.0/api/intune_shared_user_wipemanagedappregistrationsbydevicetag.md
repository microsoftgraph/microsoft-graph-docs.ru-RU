# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="fdf75-101">Действие wipeManagedAppRegistrationsByDeviceTag</span><span class="sxs-lookup"><span data-stu-id="fdf75-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="fdf75-102">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fdf75-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdf75-103">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdf75-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdf75-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdf75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdf75-105">Стирает данные о регистрации приложений с указанным тегом приложения.</span><span class="sxs-lookup"><span data-stu-id="fdf75-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fdf75-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fdf75-106">Prerequisites</span></span>
<span data-ttu-id="fdf75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdf75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdf75-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdf75-109">Permission type</span></span>|<span data-ttu-id="fdf75-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdf75-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdf75-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdf75-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fdf75-112">_Изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="fdf75-112">_varies by context_</span></span> |
| <span data-ttu-id="fdf75-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="fdf75-113">.mam</span></span> | <span data-ttu-id="fdf75-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf75-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="fdf75-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdf75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf75-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdf75-116">Not supported.</span></span>|
|<span data-ttu-id="fdf75-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdf75-117">Application</span></span>|<span data-ttu-id="fdf75-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdf75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdf75-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdf75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="fdf75-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdf75-120">Request headers</span></span>
|<span data-ttu-id="fdf75-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdf75-121">Header</span></span>|<span data-ttu-id="fdf75-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdf75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdf75-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdf75-123">Authorization</span></span>|<span data-ttu-id="fdf75-124">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="fdf75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdf75-125">Принять</span><span class="sxs-lookup"><span data-stu-id="fdf75-125">Accept</span></span>|<span data-ttu-id="fdf75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdf75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdf75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdf75-127">Request body</span></span>
<span data-ttu-id="fdf75-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdf75-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fdf75-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="fdf75-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fdf75-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdf75-130">Property</span></span>|<span data-ttu-id="fdf75-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdf75-131">Type</span></span>|<span data-ttu-id="fdf75-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdf75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf75-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="fdf75-133">deviceTag</span></span>|<span data-ttu-id="fdf75-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fdf75-134">String</span></span>|<span data-ttu-id="fdf75-135">Тег устройства</span><span class="sxs-lookup"><span data-stu-id="fdf75-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="fdf75-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdf75-136">Response</span></span>
<span data-ttu-id="fdf75-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fdf75-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fdf75-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fdf75-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdf75-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdf75-139">Request</span></span>
<span data-ttu-id="fdf75-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdf75-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="fdf75-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdf75-141">Response</span></span>
<span data-ttu-id="fdf75-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdf75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



