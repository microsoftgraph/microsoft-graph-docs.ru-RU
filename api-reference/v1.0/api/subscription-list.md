---
title: Список подписок
description: Извлечение свойств и связи webhook подписок, на основе идентификатора приложения, пользователь и роли пользователя с помощью клиента.
localization_priority: Priority
ms.openlocfilehash: 663586cc769f04be631e1f3c1bdf86bc4f798022
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850416"
---
# <a name="list-subscriptions"></a><span data-ttu-id="7edfe-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="7edfe-103">List subscriptions</span></span>

<span data-ttu-id="7edfe-104">Извлечение свойств и связи webhook подписок, на основе идентификатора приложения, пользователь и роли пользователя с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="7edfe-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7edfe-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="7edfe-105">Permissions</span></span>

<span data-ttu-id="7edfe-106">Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="7edfe-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7edfe-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7edfe-107">Permission type</span></span>  | <span data-ttu-id="7edfe-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7edfe-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="7edfe-109">[Разрешение делегированными](/graph/auth-v2-user) (рабочий или школы учетной записи)</span><span class="sxs-lookup"><span data-stu-id="7edfe-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="7edfe-110">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="7edfe-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="7edfe-111">[Разрешение делегированными](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7edfe-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="7edfe-112">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="7edfe-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="7edfe-113">Разрешение приложения</span><span class="sxs-lookup"><span data-stu-id="7edfe-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="7edfe-114">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="7edfe-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="7edfe-115">Результаты ответа зависят от контекста вызова приложения.</span><span class="sxs-lookup"><span data-stu-id="7edfe-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="7edfe-116">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="7edfe-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="7edfe-117">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="7edfe-117">Basic scenarios</span></span>

<span data-ttu-id="7edfe-118">Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи).</span><span class="sxs-lookup"><span data-stu-id="7edfe-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="7edfe-119">Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.</span><span class="sxs-lookup"><span data-stu-id="7edfe-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="7edfe-120">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="7edfe-120">Context of the calling app</span></span> | <span data-ttu-id="7edfe-121">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="7edfe-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="7edfe-122">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="7edfe-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="7edfe-123">- и -</span><span class="sxs-lookup"><span data-stu-id="7edfe-123">-and-</span></span><br/><span data-ttu-id="7edfe-124">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="7edfe-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="7edfe-125">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7edfe-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="7edfe-126">Подписки, созданные **в этом приложении** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7edfe-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="7edfe-127">Приложение вызов от имени самого (разрешений приложения).</span><span class="sxs-lookup"><span data-stu-id="7edfe-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="7edfe-128">- и -</span><span class="sxs-lookup"><span data-stu-id="7edfe-128">-and-</span></span><br/><span data-ttu-id="7edfe-129">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="7edfe-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="7edfe-130">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7edfe-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="7edfe-131">Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="7edfe-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="7edfe-132">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="7edfe-132">Advanced scenarios</span></span>

<span data-ttu-id="7edfe-133">В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях.</span><span class="sxs-lookup"><span data-stu-id="7edfe-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="7edfe-134">Например пользователю для просмотра всех подписок, созданных любого приложения от их имени.</span><span class="sxs-lookup"><span data-stu-id="7edfe-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="7edfe-135">Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.</span><span class="sxs-lookup"><span data-stu-id="7edfe-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="7edfe-136">Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7edfe-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="7edfe-137">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="7edfe-137">Context of the calling app</span></span> | <span data-ttu-id="7edfe-138">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="7edfe-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="7edfe-139">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="7edfe-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="7edfe-140">*Пользователь является без прав администратора*.</span><span class="sxs-lookup"><span data-stu-id="7edfe-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="7edfe-141">- и -</span><span class="sxs-lookup"><span data-stu-id="7edfe-141">-and-</span></span><br/><span data-ttu-id="7edfe-142">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="7edfe-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="7edfe-143">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7edfe-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="7edfe-144">Подписки, созданные в **любое приложение** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7edfe-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="7edfe-145">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="7edfe-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="7edfe-146">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="7edfe-146">*The user is an admin*.</span></span><br/><span data-ttu-id="7edfe-147">- и -</span><span class="sxs-lookup"><span data-stu-id="7edfe-147">-and-</span></span><br/><span data-ttu-id="7edfe-148">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="7edfe-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="7edfe-149">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="7edfe-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="7edfe-150">Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="7edfe-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7edfe-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7edfe-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7edfe-152">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7edfe-152">Optional query parameters</span></span>

<span data-ttu-id="7edfe-153">Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="7edfe-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7edfe-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7edfe-154">Request headers</span></span>

| <span data-ttu-id="7edfe-155">Имя</span><span class="sxs-lookup"><span data-stu-id="7edfe-155">Name</span></span>       | <span data-ttu-id="7edfe-156">Тип</span><span class="sxs-lookup"><span data-stu-id="7edfe-156">Type</span></span> | <span data-ttu-id="7edfe-157">Описание</span><span class="sxs-lookup"><span data-stu-id="7edfe-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7edfe-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="7edfe-158">Authorization</span></span>  | <span data-ttu-id="7edfe-159">string</span><span class="sxs-lookup"><span data-stu-id="7edfe-159">string</span></span>  | <span data-ttu-id="7edfe-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7edfe-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7edfe-162">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7edfe-162">Request body</span></span>

<span data-ttu-id="7edfe-163">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7edfe-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7edfe-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="7edfe-164">Response</span></span>

<span data-ttu-id="7edfe-165">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7edfe-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7edfe-166">Пример</span><span class="sxs-lookup"><span data-stu-id="7edfe-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7edfe-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="7edfe-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="7edfe-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="7edfe-168">Response</span></span>

<span data-ttu-id="7edfe-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7edfe-169">Here's an an example of the response.</span></span>  <span data-ttu-id="7edfe-170">Обратите внимание, что она может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="7edfe-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="7edfe-171">Для всех поддерживаемых свойств, подходящую для запроса и контекст вызова будет возвращен из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="7edfe-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="7edfe-172">При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.</span><span class="sxs-lookup"><span data-stu-id="7edfe-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="7edfe-173">Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="7edfe-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
