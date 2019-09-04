---
title: Перечисление подписок
description: Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ec7e5a9e52b7050cc6774b7ca6413b347a702806
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727679"
---
# <a name="list-subscriptions"></a><span data-ttu-id="ac3f4-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="ac3f4-103">List subscriptions</span></span>

<span data-ttu-id="ac3f4-104">Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac3f4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3f4-105">Permissions</span></span>

<span data-ttu-id="ac3f4-106">Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac3f4-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3f4-107">Permission type</span></span>  | <span data-ttu-id="ac3f4-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac3f4-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="ac3f4-109">[Делегированное разрешение](/graph/auth-v2-user) (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac3f4-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="ac3f4-110">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="ac3f4-111">[Делегированное разрешение](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac3f4-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="ac3f4-112">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md), или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="ac3f4-113">Разрешение приложения</span><span class="sxs-lookup"><span data-stu-id="ac3f4-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="ac3f4-114">Роль, необходимая для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="ac3f4-115">Результаты отклика основаны на контексте приложения, отправившего вызов.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="ac3f4-116">Ниже представлена сводка общих сценариев.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="ac3f4-117">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="ac3f4-117">Basic scenarios</span></span>

<span data-ttu-id="ac3f4-118">Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="ac3f4-119">В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="ac3f4-120">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="ac3f4-120">Context of the calling app</span></span> | <span data-ttu-id="ac3f4-121">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="ac3f4-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ac3f4-122">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="ac3f4-123">-и-</span><span class="sxs-lookup"><span data-stu-id="ac3f4-123">-and-</span></span><br/><span data-ttu-id="ac3f4-124">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="ac3f4-125">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ac3f4-126">Подписки, созданные **этим приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ac3f4-127">Приложение отправляет вызов от своего имени (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="ac3f4-128">-и-</span><span class="sxs-lookup"><span data-stu-id="ac3f4-128">-and-</span></span><br/><span data-ttu-id="ac3f4-129">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="ac3f4-130">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="ac3f4-131">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="ac3f4-132">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="ac3f4-132">Advanced scenarios</span></span>

<span data-ttu-id="ac3f4-133">В некоторых случаях приложению нужно получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="ac3f4-134">Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="ac3f4-135">Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="ac3f4-136">В таких сценариях требуется делегированное разрешение Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="ac3f4-137">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="ac3f4-137">Context of the calling app</span></span> | <span data-ttu-id="ac3f4-138">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="ac3f4-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ac3f4-139">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ac3f4-140">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="ac3f4-141">-и-</span><span class="sxs-lookup"><span data-stu-id="ac3f4-141">-and-</span></span><br/><span data-ttu-id="ac3f4-142">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac3f4-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ac3f4-143">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ac3f4-144">Подписки, созданные **любым приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ac3f4-145">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ac3f4-146">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-146">*The user is an admin*.</span></span><br/><span data-ttu-id="ac3f4-147">-и-</span><span class="sxs-lookup"><span data-stu-id="ac3f4-147">-and-</span></span><br/><span data-ttu-id="ac3f4-148">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac3f4-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ac3f4-149">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="ac3f4-150">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac3f4-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac3f4-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac3f4-152">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ac3f4-152">Optional query parameters</span></span>

<span data-ttu-id="ac3f4-153">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac3f4-154">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac3f4-154">Request headers</span></span>

| <span data-ttu-id="ac3f4-155">Имя</span><span class="sxs-lookup"><span data-stu-id="ac3f4-155">Name</span></span>       | <span data-ttu-id="ac3f4-156">Тип</span><span class="sxs-lookup"><span data-stu-id="ac3f4-156">Type</span></span> | <span data-ttu-id="ac3f4-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ac3f4-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ac3f4-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac3f4-158">Authorization</span></span>  | <span data-ttu-id="ac3f4-159">string</span><span class="sxs-lookup"><span data-stu-id="ac3f4-159">string</span></span>  | <span data-ttu-id="ac3f4-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac3f4-162">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac3f4-162">Request body</span></span>

<span data-ttu-id="ac3f4-163">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac3f4-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac3f4-164">Response</span></span>

<span data-ttu-id="ac3f4-165">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac3f4-166">Пример</span><span class="sxs-lookup"><span data-stu-id="ac3f4-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ac3f4-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac3f4-167">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ac3f4-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac3f4-168">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac3f4-169">C#</span><span class="sxs-lookup"><span data-stu-id="ac3f4-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac3f4-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac3f4-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac3f4-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac3f4-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ac3f4-172">Java</span><span class="sxs-lookup"><span data-stu-id="ac3f4-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ac3f4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac3f4-173">Response</span></span>

<span data-ttu-id="ac3f4-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-174">Here's an an example of the response.</span></span>  <span data-ttu-id="ac3f4-175">Обратите внимание, что он может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-175">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="ac3f4-176">При фактическом вызове будут возвращены все поддерживаемые свойства, соответствующие запросу и контексту вызова.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-176">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->

<span data-ttu-id="ac3f4-177">Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="ac3f4-177">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="ac3f4-178">Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="ac3f4-178">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
