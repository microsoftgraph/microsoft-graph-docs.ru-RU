# <a name="list-subscriptions"></a><span data-ttu-id="db997-101">Перечислить подписки</span><span class="sxs-lookup"><span data-stu-id="db997-101">List subscriptions</span></span>

<span data-ttu-id="db997-102">Выводит свойства и отношения подписок типа веб-перехватчиков на основе идентификатора приложения, пользователя и роли пользователя по отношению к клиенту.</span><span class="sxs-lookup"><span data-stu-id="db997-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="db997-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db997-103">Permissions</span></span>

<span data-ttu-id="db997-104">Этот API поддерживает следующие области разрешений. Для получения дополнительных сведений, а также чтобы узнать, как выбирать разрешения, см. [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="db997-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="db997-105">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db997-105">Permission type</span></span>  | <span data-ttu-id="db997-106">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db997-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="db997-107">[Делегированные](../../../concepts/auth_v2_user.md) (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db997-107">Delegated (work or school account)</span></span> | <span data-ttu-id="db997-108">Роли, необходимые для [создания подписки](subscription_get.md) или Subscriptions.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="db997-108">Role required to [create subscription](subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| <span data-ttu-id="db997-109">[Делегированные](../../../concepts/auth_v2_user.md) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db997-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db997-110">Роли, необходимые для [создания подписки](./subscription_get.md) или Subscriptions.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="db997-110">Role required to [create subscription](./subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| [<span data-ttu-id="db997-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="db997-111">Application</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="db997-112">Роли, необходимые для [создания подписки](./subscription_get.md).</span><span class="sxs-lookup"><span data-stu-id="db997-112">Role required to [create subscription](./subscription_get.md).</span></span> |

<span data-ttu-id="db997-113">Результаты ответов определяются по контексту вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="db997-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="db997-114">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="db997-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="db997-115">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="db997-115">Basic planning scenarios</span></span>

<span data-ttu-id="db997-116">Чаще всего приложение пытается показать подписки, которые оно изначально создало для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочие/учебные учетные записи).</span><span class="sxs-lookup"><span data-stu-id="db997-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="db997-117">Эти сценарии не требуют каких-либо специальных разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="db997-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="db997-118">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="db997-118">Context of the calling app</span></span> | <span data-ttu-id="db997-119">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="db997-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="db997-120">Приложение вызывает от имени выполнившего вход пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="db997-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="db997-121">- и -</span><span class="sxs-lookup"><span data-stu-id="db997-121">and</span></span><br/><span data-ttu-id="db997-122">Приложение изначально имеет разрешение, которое необходимо, чтобы [создать список](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="db997-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="db997-123">Примечание. Это применимо к личным учетным записям Майкрософт и рабочим/учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="db997-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="db997-124">Подписки, созданные **этим приложением** только для выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="db997-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="db997-125">Приложение вызывает от своего имени (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="db997-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="db997-126">- и -</span><span class="sxs-lookup"><span data-stu-id="db997-126">and</span></span><br/><span data-ttu-id="db997-127">Приложение изначально имеет разрешение, которое необходимо, чтобы [создать список](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="db997-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="db997-128">Примечание. Это применимо к только рабочим/учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="db997-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="db997-129">Подписки, созданные **этим приложением** для себя или для какого-либо пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="db997-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="db997-130">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="db997-130">Advanced save scenarios</span></span>

<span data-ttu-id="db997-131">В некоторых случаях приложения пытается показать подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="db997-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="db997-132">Например, пользователю необходимо просмотреть все подписки, созданные каким-либо приложением от его имени.</span><span class="sxs-lookup"><span data-stu-id="db997-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="db997-133">Или администратору может потребоваться просмотреть все подписки от всех приложений в его каталоге.</span><span class="sxs-lookup"><span data-stu-id="db997-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="db997-134">Для таких сценариев требуется делегированное разрешение Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="db997-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="db997-135">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="db997-135">Context of the calling app</span></span> | <span data-ttu-id="db997-136">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="db997-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="db997-137">Приложение вызывает от имени выполнившего вход пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="db997-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="db997-138">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="db997-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="db997-139">- и -</span><span class="sxs-lookup"><span data-stu-id="db997-139">and</span></span><br/><span data-ttu-id="db997-140">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="db997-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="db997-141">Примечание. Это применимо к личным учетным записям Майкрософт и рабочим/учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="db997-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="db997-142">Подписки, созданные **каким-либо приложением** только для выполнившего вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="db997-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="db997-143">Приложение вызывает от имени выполнившего вход пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="db997-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="db997-144">В списке приложений выберите пункт *Администратор*.</span><span class="sxs-lookup"><span data-stu-id="db997-144">*The user is an admin*.</span></span><br/><span data-ttu-id="db997-145">- и -</span><span class="sxs-lookup"><span data-stu-id="db997-145">and</span></span><br/><span data-ttu-id="db997-146">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="db997-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="db997-147">Примечание. Это применимо к только рабочим/учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="db997-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="db997-148">Подписки, созданные **каким-либо приложением** для **какого-либо пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="db997-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db997-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db997-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db997-150">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db997-150">Optional query parameters</span></span>

<span data-ttu-id="db997-151">Этот метод не поддерживает [Параметры запроса OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="db997-151">This method does not support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="db997-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db997-152">Request headers</span></span>

| <span data-ttu-id="db997-153">Имя</span><span class="sxs-lookup"><span data-stu-id="db997-153">Name</span></span>       | <span data-ttu-id="db997-154">Тип</span><span class="sxs-lookup"><span data-stu-id="db997-154">Type</span></span> | <span data-ttu-id="db997-155">Описание</span><span class="sxs-lookup"><span data-stu-id="db997-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db997-156">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db997-156">Authorization</span></span>  | <span data-ttu-id="db997-157">строка</span><span class="sxs-lookup"><span data-stu-id="db997-157">string</span></span>  | <span data-ttu-id="db997-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db997-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db997-160">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db997-160">Request body</span></span>

<span data-ttu-id="db997-161">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db997-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db997-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="db997-162">Response</span></span>

<span data-ttu-id="db997-163">При успешном выполнении этот метод возвращает `200 OK` код ответа и список [   объектов](../resources/subscription.md)  в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="db997-163">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db997-164">Пример</span><span class="sxs-lookup"><span data-stu-id="db997-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db997-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="db997-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="db997-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="db997-166">Response</span></span>

<span data-ttu-id="db997-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db997-167">Here's an excerpt of the response:</span></span>  <span data-ttu-id="db997-168">Обратите внимание, что он может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="db997-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="db997-169">Все поддерживаемые свойства, относящиеся к запросу и контексту вызова, будут возвращены из фактического вызова.</span><span class="sxs-lookup"><span data-stu-id="db997-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="db997-170">При возврате нескольких страниц данных ответ включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="db997-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="db997-171">Для получения дополнительных сведений см. [Постраничный просмотр данных Microsoft Graph в вашем приложении](../../../concepts/paging.md).</span><span class="sxs-lookup"><span data-stu-id="db997-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
