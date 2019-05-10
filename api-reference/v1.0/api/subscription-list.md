---
title: Перечисление подписок
description: Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 2255d9b4b21809a082ff59ba40f49d9c557620d6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603262"
---
# <a name="list-subscriptions"></a><span data-ttu-id="dbbe3-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="dbbe3-103">List subscriptions</span></span>

<span data-ttu-id="dbbe3-104">Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbbe3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbbe3-105">Permissions</span></span>

<span data-ttu-id="dbbe3-106">Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dbbe3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbbe3-107">Permission type</span></span>  | <span data-ttu-id="dbbe3-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="dbbe3-109">[Делегированное разрешение](/graph/auth-v2-user) (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="dbbe3-110">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="dbbe3-111">[Делегированное разрешение](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbbe3-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="dbbe3-112">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="dbbe3-113">Разрешение приложения</span><span class="sxs-lookup"><span data-stu-id="dbbe3-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="dbbe3-114">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="dbbe3-115">Результаты отклика основаны на контексте приложения, отправившего вызов.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="dbbe3-116">Ниже представлена сводка общих сценариев.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="dbbe3-117">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="dbbe3-117">Basic scenarios</span></span>

<span data-ttu-id="dbbe3-118">Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="dbbe3-119">В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="dbbe3-120">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="dbbe3-120">Context of the calling app</span></span> | <span data-ttu-id="dbbe3-121">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="dbbe3-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="dbbe3-122">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="dbbe3-123">-и-</span><span class="sxs-lookup"><span data-stu-id="dbbe3-123">-and-</span></span><br/><span data-ttu-id="dbbe3-124">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="dbbe3-125">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="dbbe3-126">Подписки, созданные **этим приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="dbbe3-127">Приложение отправляет вызов от своего имени (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="dbbe3-128">-и-</span><span class="sxs-lookup"><span data-stu-id="dbbe3-128">-and-</span></span><br/><span data-ttu-id="dbbe3-129">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="dbbe3-130">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="dbbe3-131">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="dbbe3-132">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="dbbe3-132">Advanced scenarios</span></span>

<span data-ttu-id="dbbe3-133">В некоторых случаях приложению нужно получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="dbbe3-134">Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="dbbe3-135">Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="dbbe3-136">В таких сценариях требуется делегированное разрешение Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="dbbe3-137">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="dbbe3-137">Context of the calling app</span></span> | <span data-ttu-id="dbbe3-138">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="dbbe3-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="dbbe3-139">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="dbbe3-140">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="dbbe3-141">-и-</span><span class="sxs-lookup"><span data-stu-id="dbbe3-141">-and-</span></span><br/><span data-ttu-id="dbbe3-142">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbe3-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="dbbe3-143">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="dbbe3-144">Подписки, созданные **любым приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="dbbe3-145">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="dbbe3-146">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-146">*The user is an admin*.</span></span><br/><span data-ttu-id="dbbe3-147">-и-</span><span class="sxs-lookup"><span data-stu-id="dbbe3-147">-and-</span></span><br/><span data-ttu-id="dbbe3-148">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbe3-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="dbbe3-149">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="dbbe3-150">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbbe3-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbbe3-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbbe3-152">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dbbe3-152">Optional query parameters</span></span>

<span data-ttu-id="dbbe3-153">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbbe3-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbbe3-154">Request headers</span></span>

| <span data-ttu-id="dbbe3-155">Имя</span><span class="sxs-lookup"><span data-stu-id="dbbe3-155">Name</span></span>       | <span data-ttu-id="dbbe3-156">Тип</span><span class="sxs-lookup"><span data-stu-id="dbbe3-156">Type</span></span> | <span data-ttu-id="dbbe3-157">Описание</span><span class="sxs-lookup"><span data-stu-id="dbbe3-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbbe3-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbbe3-158">Authorization</span></span>  | <span data-ttu-id="dbbe3-159">string</span><span class="sxs-lookup"><span data-stu-id="dbbe3-159">string</span></span>  | <span data-ttu-id="dbbe3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbbe3-162">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbbe3-162">Request body</span></span>

<span data-ttu-id="dbbe3-163">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbbe3-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbbe3-164">Response</span></span>

<span data-ttu-id="dbbe3-165">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbbe3-166">Пример</span><span class="sxs-lookup"><span data-stu-id="dbbe3-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dbbe3-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbbe3-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="dbbe3-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbbe3-168">Response</span></span>

<span data-ttu-id="dbbe3-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-169">Here's an an example of the response.</span></span>  <span data-ttu-id="dbbe3-170">Обратите внимание, что он может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="dbbe3-171">При фактическом вызове будут возвращены все поддерживаемые свойства, соответствующие запросу и контексту вызова.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dbbe3-172">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="dbbe3-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dbbe3-173">C#</span><span class="sxs-lookup"><span data-stu-id="dbbe3-173">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbbe3-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="dbbe3-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

<span data-ttu-id="dbbe3-175">Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="dbbe3-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="dbbe3-176">Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="dbbe3-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
