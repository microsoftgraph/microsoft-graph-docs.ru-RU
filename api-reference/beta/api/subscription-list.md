---
title: Список подписок
description: " сценарии ниже для получения дополнительных сведений см."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e7b6c618c35aa9952673b79f238777a71bc41f6a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928782"
---
# <a name="list-subscriptions"></a><span data-ttu-id="19b05-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="19b05-103">List subscriptions</span></span>

> <span data-ttu-id="19b05-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19b05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19b05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19b05-106">Получение списка webhook подписки.</span><span class="sxs-lookup"><span data-stu-id="19b05-106">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="19b05-107">Содержимое ответа зависит от контекста, в котором вызов приложения; сценарии ниже для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="19b05-107">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="19b05-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19b05-108">Permissions</span></span>

<span data-ttu-id="19b05-109">Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="19b05-109">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19b05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19b05-110">Permission type</span></span>  | <span data-ttu-id="19b05-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19b05-111">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="19b05-112">[Делегирование](/graph/auth-v2-user) (рабочий или школы учетной записи)</span><span class="sxs-lookup"><span data-stu-id="19b05-112">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="19b05-113">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="19b05-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="19b05-114">[Делегирование](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19b05-114">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="19b05-115">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="19b05-115">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="19b05-116">Application</span><span class="sxs-lookup"><span data-stu-id="19b05-116">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="19b05-117">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="19b05-117">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="19b05-118">Результаты ответа зависят от контекста вызова приложения.</span><span class="sxs-lookup"><span data-stu-id="19b05-118">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="19b05-119">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="19b05-119">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="19b05-120">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="19b05-120">Basic scenarios</span></span>

<span data-ttu-id="19b05-121">Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи).</span><span class="sxs-lookup"><span data-stu-id="19b05-121">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="19b05-122">Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.</span><span class="sxs-lookup"><span data-stu-id="19b05-122">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="19b05-123">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="19b05-123">Context of the calling app</span></span> | <span data-ttu-id="19b05-124">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="19b05-124">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="19b05-125">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="19b05-125">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="19b05-126">- и -</span><span class="sxs-lookup"><span data-stu-id="19b05-126">-and-</span></span><br/><span data-ttu-id="19b05-127">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="19b05-127">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="19b05-128">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="19b05-128">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="19b05-129">Подписки, созданные **в этом приложении** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b05-129">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="19b05-130">Приложение вызов от имени самого (разрешений приложения).</span><span class="sxs-lookup"><span data-stu-id="19b05-130">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="19b05-131">- и -</span><span class="sxs-lookup"><span data-stu-id="19b05-131">-and-</span></span><br/><span data-ttu-id="19b05-132">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="19b05-132">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="19b05-133">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="19b05-133">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="19b05-134">Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="19b05-134">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="19b05-135">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="19b05-135">Advanced scenarios</span></span>

<span data-ttu-id="19b05-136">В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях.</span><span class="sxs-lookup"><span data-stu-id="19b05-136">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="19b05-137">Например пользователю для просмотра всех подписок, созданных любого приложения от их имени.</span><span class="sxs-lookup"><span data-stu-id="19b05-137">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="19b05-138">Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.</span><span class="sxs-lookup"><span data-stu-id="19b05-138">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="19b05-139">Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.</span><span class="sxs-lookup"><span data-stu-id="19b05-139">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="19b05-140">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="19b05-140">Context of the calling app</span></span> | <span data-ttu-id="19b05-141">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="19b05-141">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="19b05-142">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="19b05-142">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="19b05-143">*Пользователь является без прав администратора*.</span><span class="sxs-lookup"><span data-stu-id="19b05-143">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="19b05-144">- и -</span><span class="sxs-lookup"><span data-stu-id="19b05-144">-and-</span></span><br/><span data-ttu-id="19b05-145">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b05-145">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="19b05-146">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="19b05-146">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="19b05-147">Подписки, созданные в **любое приложение** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="19b05-147">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="19b05-148">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="19b05-148">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="19b05-149">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="19b05-149">*The user is an admin*.</span></span><br/><span data-ttu-id="19b05-150">- и -</span><span class="sxs-lookup"><span data-stu-id="19b05-150">-and-</span></span><br/><span data-ttu-id="19b05-151">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="19b05-151">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="19b05-152">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="19b05-152">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="19b05-153">Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="19b05-153">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b05-154">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19b05-154">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19b05-155">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19b05-155">Optional query parameters</span></span>

<span data-ttu-id="19b05-156">Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="19b05-156">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19b05-157">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19b05-157">Request headers</span></span>

| <span data-ttu-id="19b05-158">Имя</span><span class="sxs-lookup"><span data-stu-id="19b05-158">Name</span></span>       | <span data-ttu-id="19b05-159">Тип</span><span class="sxs-lookup"><span data-stu-id="19b05-159">Type</span></span> | <span data-ttu-id="19b05-160">Описание</span><span class="sxs-lookup"><span data-stu-id="19b05-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19b05-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b05-161">Authorization</span></span>  | <span data-ttu-id="19b05-162">строка</span><span class="sxs-lookup"><span data-stu-id="19b05-162">string</span></span>  | <span data-ttu-id="19b05-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19b05-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19b05-165">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19b05-165">Request body</span></span>

<span data-ttu-id="19b05-166">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19b05-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19b05-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b05-167">Response</span></span>

<span data-ttu-id="19b05-168">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19b05-168">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b05-169">Пример</span><span class="sxs-lookup"><span data-stu-id="19b05-169">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19b05-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="19b05-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="19b05-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b05-171">Response</span></span>

<span data-ttu-id="19b05-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19b05-172">Here is an example of the response.</span></span> <span data-ttu-id="19b05-173">Примечание: Для краткости может усекаться ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="19b05-173">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="19b05-174">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19b05-174">All of the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
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

<span data-ttu-id="19b05-175">При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.</span><span class="sxs-lookup"><span data-stu-id="19b05-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="19b05-176">Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="19b05-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
