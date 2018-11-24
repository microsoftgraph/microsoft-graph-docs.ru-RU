# <a name="list-subscriptions"></a><span data-ttu-id="a8bdc-101">Список подписок</span><span class="sxs-lookup"><span data-stu-id="a8bdc-101">List subscriptions</span></span>

<span data-ttu-id="a8bdc-102">Извлечение свойств и связи webhook подписок, на основе идентификатора приложения, пользователь и роли пользователя с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8bdc-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8bdc-103">Permissions</span></span>

<span data-ttu-id="a8bdc-104">Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](../../../concepts/permissions_reference.md)</span><span class="sxs-lookup"><span data-stu-id="a8bdc-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a8bdc-105">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8bdc-105">Permission type</span></span>  | <span data-ttu-id="a8bdc-106">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8bdc-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="a8bdc-107">[Разрешение делегированными](../../../concepts/auth_v2_user.md) (рабочий или школы учетной записи)</span><span class="sxs-lookup"><span data-stu-id="a8bdc-107">[Delegated permission](../../../concepts/auth_v2_user.md) (work or school account)</span></span> | <span data-ttu-id="a8bdc-108">Роли, необходимые для [создания подписки](subscription_post_subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-108">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="a8bdc-109">[Разрешение делегированными](../../../concepts/auth_v2_user.md) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8bdc-109">[Delegated permission](../../../concepts/auth_v2_user.md) (personal Microsoft account)</span></span> | <span data-ttu-id="a8bdc-110">Роли, необходимые для [создания подписки](subscription_post_subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-110">Role required to [create subscription](subscription_post_subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="a8bdc-111">Разрешение приложения</span><span class="sxs-lookup"><span data-stu-id="a8bdc-111">Application permission</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="a8bdc-112">Роли, необходимые для [создания подписки](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-112">Role required to [create subscription](subscription_post_subscriptions.md).</span></span> |

<span data-ttu-id="a8bdc-113">Результаты ответа зависят от контекста вызова приложения.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="a8bdc-114">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="a8bdc-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="a8bdc-115">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="a8bdc-115">Basic scenarios</span></span>

<span data-ttu-id="a8bdc-116">Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="a8bdc-117">Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="a8bdc-118">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="a8bdc-118">Context of the calling app</span></span> | <span data-ttu-id="a8bdc-119">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="a8bdc-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="a8bdc-120">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="a8bdc-121">- и -</span><span class="sxs-lookup"><span data-stu-id="a8bdc-121">-and-</span></span><br/><span data-ttu-id="a8bdc-122">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="a8bdc-123">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="a8bdc-124">Подписки, созданные **в этом приложении** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="a8bdc-125">Приложение вызов от имени самого (разрешений приложения).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="a8bdc-126">- и -</span><span class="sxs-lookup"><span data-stu-id="a8bdc-126">-and-</span></span><br/><span data-ttu-id="a8bdc-127">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription_post_subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="a8bdc-128">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="a8bdc-129">Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="a8bdc-130">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="a8bdc-130">Advanced scenarios</span></span>

<span data-ttu-id="a8bdc-131">В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="a8bdc-132">Например пользователю для просмотра всех подписок, созданных любого приложения от их имени.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="a8bdc-133">Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="a8bdc-134">Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="a8bdc-135">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="a8bdc-135">Context of the calling app</span></span> | <span data-ttu-id="a8bdc-136">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="a8bdc-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="a8bdc-137">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="a8bdc-138">*Пользователь является без прав администратора*.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="a8bdc-139">- и -</span><span class="sxs-lookup"><span data-stu-id="a8bdc-139">-and-</span></span><br/><span data-ttu-id="a8bdc-140">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bdc-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="a8bdc-141">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="a8bdc-142">Подписки, созданные в **любое приложение** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="a8bdc-143">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="a8bdc-144">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-144">*The user is an admin*.</span></span><br/><span data-ttu-id="a8bdc-145">- и -</span><span class="sxs-lookup"><span data-stu-id="a8bdc-145">-and-</span></span><br/><span data-ttu-id="a8bdc-146">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bdc-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="a8bdc-147">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="a8bdc-148">Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8bdc-149">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8bdc-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8bdc-150">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8bdc-150">Optional query parameters</span></span>

<span data-ttu-id="a8bdc-151">Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-151">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8bdc-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8bdc-152">Request headers</span></span>

| <span data-ttu-id="a8bdc-153">Имя</span><span class="sxs-lookup"><span data-stu-id="a8bdc-153">Name</span></span>       | <span data-ttu-id="a8bdc-154">Тип</span><span class="sxs-lookup"><span data-stu-id="a8bdc-154">Type</span></span> | <span data-ttu-id="a8bdc-155">Описание</span><span class="sxs-lookup"><span data-stu-id="a8bdc-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8bdc-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8bdc-156">Authorization</span></span>  | <span data-ttu-id="a8bdc-157">string</span><span class="sxs-lookup"><span data-stu-id="a8bdc-157">string</span></span>  | <span data-ttu-id="a8bdc-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8bdc-160">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8bdc-160">Request body</span></span>

<span data-ttu-id="a8bdc-161">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8bdc-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8bdc-162">Response</span></span>

<span data-ttu-id="a8bdc-163">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-163">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bdc-164">Пример</span><span class="sxs-lookup"><span data-stu-id="a8bdc-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a8bdc-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8bdc-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="a8bdc-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8bdc-166">Response</span></span>

<span data-ttu-id="a8bdc-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-167">Here's an an example of the response.</span></span>  <span data-ttu-id="a8bdc-168">Обратите внимание, что она может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="a8bdc-169">Для всех поддерживаемых свойств, подходящую для запроса и контекст вызова будет возвращен из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="a8bdc-170">При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.</span><span class="sxs-lookup"><span data-stu-id="a8bdc-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="a8bdc-171">Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](../../../concepts/paging.md).</span><span class="sxs-lookup"><span data-stu-id="a8bdc-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
