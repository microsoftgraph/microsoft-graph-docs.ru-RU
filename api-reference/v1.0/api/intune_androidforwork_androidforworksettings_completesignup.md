# <a name="completesignup-action"></a><span data-ttu-id="422ea-101">Действие completeSignup</span><span class="sxs-lookup"><span data-stu-id="422ea-101">completeSignup action</span></span>

> <span data-ttu-id="422ea-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="422ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="422ea-103">Завершает поток регистрации для управления Android for Work.</span><span class="sxs-lookup"><span data-stu-id="422ea-103">Completes the sign-up flow for Android for Work management.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="422ea-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="422ea-104">Prerequisites</span></span>
<span data-ttu-id="422ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="422ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="422ea-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422ea-107">Permission type</span></span>|<span data-ttu-id="422ea-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="422ea-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="422ea-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422ea-109">Delegated (work or school account)</span></span>|<span data-ttu-id="422ea-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422ea-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="422ea-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422ea-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="422ea-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422ea-112">Not supported.</span></span>|
|<span data-ttu-id="422ea-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="422ea-113">Application</span></span>|<span data-ttu-id="422ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422ea-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="422ea-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422ea-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/completeSignup
```

## <a name="request-headers"></a><span data-ttu-id="422ea-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="422ea-116">Request headers</span></span>
|<span data-ttu-id="422ea-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="422ea-117">Header</span></span>|<span data-ttu-id="422ea-118">Значение</span><span class="sxs-lookup"><span data-stu-id="422ea-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="422ea-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="422ea-119">Authorization</span></span>|<span data-ttu-id="422ea-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422ea-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="422ea-121">Accept</span><span class="sxs-lookup"><span data-stu-id="422ea-121">Accept</span></span>|<span data-ttu-id="422ea-122">application/json</span><span class="sxs-lookup"><span data-stu-id="422ea-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="422ea-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="422ea-123">Request body</span></span>
<span data-ttu-id="422ea-124">В текст запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="422ea-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="422ea-125">В таблице ниже приведены параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="422ea-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="422ea-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="422ea-126">Property</span></span>|<span data-ttu-id="422ea-127">Тип</span><span class="sxs-lookup"><span data-stu-id="422ea-127">Type</span></span>|<span data-ttu-id="422ea-128">Описание</span><span class="sxs-lookup"><span data-stu-id="422ea-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="422ea-129">enterpriseToken</span><span class="sxs-lookup"><span data-stu-id="422ea-129">enterpriseToken</span></span>|<span data-ttu-id="422ea-130">String</span><span class="sxs-lookup"><span data-stu-id="422ea-130">String</span></span>|<span data-ttu-id="422ea-131">Маркер Enterprise, который добавляется к URL-адресу обратного вызова после успешной регистрации.</span><span class="sxs-lookup"><span data-stu-id="422ea-131">The Enterprise token appended to the callback URL after successfully completing sign-up.</span></span>|



## <a name="response"></a><span data-ttu-id="422ea-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="422ea-132">Response</span></span>
<span data-ttu-id="422ea-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="422ea-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="422ea-134">Пример</span><span class="sxs-lookup"><span data-stu-id="422ea-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="422ea-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="422ea-135">Request</span></span>
<span data-ttu-id="422ea-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422ea-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings/completeSignup

Content-type: application/json
Content-length: 51

{
  "enterpriseToken": "Enterprise Token value"
}
```

### <a name="response"></a><span data-ttu-id="422ea-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="422ea-137">Response</span></span>
<span data-ttu-id="422ea-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="422ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



