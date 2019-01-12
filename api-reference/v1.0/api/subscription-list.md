---
title: Список подписок
description: Извлечение свойств и связи webhook подписок, на основе идентификатора приложения, пользователь и роли пользователя с помощью клиента.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: c2e9446721f4390341c33f8b976893e4b1ab14be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972938"
---
# <a name="list-subscriptions"></a><span data-ttu-id="6248b-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="6248b-103">List subscriptions</span></span>

<span data-ttu-id="6248b-104">Извлечение свойств и связи webhook подписок, на основе идентификатора приложения, пользователь и роли пользователя с помощью клиента.</span><span class="sxs-lookup"><span data-stu-id="6248b-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6248b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6248b-105">Permissions</span></span>

<span data-ttu-id="6248b-106">Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="6248b-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6248b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6248b-107">Permission type</span></span>  | <span data-ttu-id="6248b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6248b-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="6248b-109">[Разрешение делегированными](/graph/auth-v2-user) (рабочий или школы учетной записи)</span><span class="sxs-lookup"><span data-stu-id="6248b-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="6248b-110">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="6248b-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="6248b-111">[Разрешение делегированными](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6248b-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="6248b-112">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="6248b-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="6248b-113">Разрешение приложения</span><span class="sxs-lookup"><span data-stu-id="6248b-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="6248b-114">Роли, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="6248b-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="6248b-115">Результаты ответа зависят от контекста вызова приложения.</span><span class="sxs-lookup"><span data-stu-id="6248b-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="6248b-116">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="6248b-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="6248b-117">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="6248b-117">Basic scenarios</span></span>

<span data-ttu-id="6248b-118">Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи).</span><span class="sxs-lookup"><span data-stu-id="6248b-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="6248b-119">Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.</span><span class="sxs-lookup"><span data-stu-id="6248b-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="6248b-120">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="6248b-120">Context of the calling app</span></span> | <span data-ttu-id="6248b-121">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="6248b-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="6248b-122">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="6248b-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="6248b-123">- и -</span><span class="sxs-lookup"><span data-stu-id="6248b-123">-and-</span></span><br/><span data-ttu-id="6248b-124">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="6248b-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="6248b-125">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="6248b-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="6248b-126">Подписки, созданные **в этом приложении** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6248b-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="6248b-127">Приложение вызов от имени самого (разрешений приложения).</span><span class="sxs-lookup"><span data-stu-id="6248b-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="6248b-128">- и -</span><span class="sxs-lookup"><span data-stu-id="6248b-128">-and-</span></span><br/><span data-ttu-id="6248b-129">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="6248b-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="6248b-130">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="6248b-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="6248b-131">Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6248b-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="6248b-132">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="6248b-132">Advanced scenarios</span></span>

<span data-ttu-id="6248b-133">В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях.</span><span class="sxs-lookup"><span data-stu-id="6248b-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="6248b-134">Например пользователю для просмотра всех подписок, созданных любого приложения от их имени.</span><span class="sxs-lookup"><span data-stu-id="6248b-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="6248b-135">Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.</span><span class="sxs-lookup"><span data-stu-id="6248b-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="6248b-136">Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6248b-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="6248b-137">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="6248b-137">Context of the calling app</span></span> | <span data-ttu-id="6248b-138">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="6248b-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="6248b-139">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="6248b-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="6248b-140">*Пользователь является без прав администратора*.</span><span class="sxs-lookup"><span data-stu-id="6248b-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="6248b-141">- и -</span><span class="sxs-lookup"><span data-stu-id="6248b-141">-and-</span></span><br/><span data-ttu-id="6248b-142">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="6248b-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="6248b-143">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="6248b-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="6248b-144">Подписки, созданные в **любое приложение** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6248b-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="6248b-145">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="6248b-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="6248b-146">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="6248b-146">*The user is an admin*.</span></span><br/><span data-ttu-id="6248b-147">- и -</span><span class="sxs-lookup"><span data-stu-id="6248b-147">-and-</span></span><br/><span data-ttu-id="6248b-148">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="6248b-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="6248b-149">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="6248b-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="6248b-150">Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6248b-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6248b-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6248b-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6248b-152">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6248b-152">Optional query parameters</span></span>

<span data-ttu-id="6248b-153">Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="6248b-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6248b-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6248b-154">Request headers</span></span>

| <span data-ttu-id="6248b-155">Имя</span><span class="sxs-lookup"><span data-stu-id="6248b-155">Name</span></span>       | <span data-ttu-id="6248b-156">Тип</span><span class="sxs-lookup"><span data-stu-id="6248b-156">Type</span></span> | <span data-ttu-id="6248b-157">Описание</span><span class="sxs-lookup"><span data-stu-id="6248b-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6248b-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="6248b-158">Authorization</span></span>  | <span data-ttu-id="6248b-159">строка</span><span class="sxs-lookup"><span data-stu-id="6248b-159">string</span></span>  | <span data-ttu-id="6248b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6248b-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6248b-162">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6248b-162">Request body</span></span>

<span data-ttu-id="6248b-163">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6248b-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6248b-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="6248b-164">Response</span></span>

<span data-ttu-id="6248b-165">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6248b-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6248b-166">Пример</span><span class="sxs-lookup"><span data-stu-id="6248b-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6248b-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="6248b-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="6248b-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="6248b-168">Response</span></span>

<span data-ttu-id="6248b-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6248b-169">Here's an an example of the response.</span></span>  <span data-ttu-id="6248b-170">Обратите внимание, что она может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="6248b-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="6248b-171">Для всех поддерживаемых свойств, подходящую для запроса и контекст вызова будет возвращен из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="6248b-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="6248b-172">При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.</span><span class="sxs-lookup"><span data-stu-id="6248b-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="6248b-173">Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="6248b-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
