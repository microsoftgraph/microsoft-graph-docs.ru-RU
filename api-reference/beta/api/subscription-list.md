---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 97fed1e7271ab39bad64f1bb56ac1696e351b4cf
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722295"
---
# <a name="list-subscriptions"></a><span data-ttu-id="32999-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="32999-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32999-104">Получение списка подписок на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="32999-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="32999-105">Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="32999-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="32999-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32999-106">Permissions</span></span>

<span data-ttu-id="32999-107">Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32999-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32999-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32999-108">Permission type</span></span>  | <span data-ttu-id="32999-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32999-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="32999-110">[Делегированный](/graph/auth-v2-user) (Рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32999-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="32999-111">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="32999-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="32999-112">[Делегированный](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32999-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="32999-113">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="32999-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="32999-114">Application</span><span class="sxs-lookup"><span data-stu-id="32999-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="32999-115">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="32999-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="32999-116">Результаты отклика основаны на контексте приложения, отправившего вызов.</span><span class="sxs-lookup"><span data-stu-id="32999-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="32999-117">Ниже представлена сводка общих сценариев.</span><span class="sxs-lookup"><span data-stu-id="32999-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="32999-118">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="32999-118">Basic scenarios</span></span>

<span data-ttu-id="32999-119">Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей).</span><span class="sxs-lookup"><span data-stu-id="32999-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="32999-120">В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="32999-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="32999-121">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="32999-121">Context of the calling app</span></span> | <span data-ttu-id="32999-122">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="32999-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="32999-123">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="32999-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="32999-124">-и-</span><span class="sxs-lookup"><span data-stu-id="32999-124">-and-</span></span><br/><span data-ttu-id="32999-125">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="32999-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="32999-126">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="32999-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="32999-127">Подписки, созданные **этим приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="32999-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="32999-128">Приложение отправляет вызов от своего имени (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="32999-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="32999-129">-и-</span><span class="sxs-lookup"><span data-stu-id="32999-129">-and-</span></span><br/><span data-ttu-id="32999-130">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="32999-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="32999-131">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="32999-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="32999-132">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="32999-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="32999-133">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="32999-133">Advanced scenarios</span></span>

<span data-ttu-id="32999-134">В некоторых случаях приложению нужно получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="32999-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="32999-135">Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени.</span><span class="sxs-lookup"><span data-stu-id="32999-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="32999-136">Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="32999-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="32999-137">В таких сценариях требуется делегированное разрешение Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="32999-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="32999-138">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="32999-138">Context of the calling app</span></span> | <span data-ttu-id="32999-139">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="32999-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="32999-140">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="32999-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="32999-141">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="32999-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="32999-142">-и-</span><span class="sxs-lookup"><span data-stu-id="32999-142">-and-</span></span><br/><span data-ttu-id="32999-143">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="32999-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="32999-144">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="32999-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="32999-145">Подписки, созданные **любым приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="32999-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="32999-146">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="32999-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="32999-147">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="32999-147">*The user is an admin*.</span></span><br/><span data-ttu-id="32999-148">-и-</span><span class="sxs-lookup"><span data-stu-id="32999-148">-and-</span></span><br/><span data-ttu-id="32999-149">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="32999-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="32999-150">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="32999-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="32999-151">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="32999-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32999-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32999-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32999-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32999-153">Optional query parameters</span></span>

<span data-ttu-id="32999-154">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="32999-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32999-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32999-155">Request headers</span></span>

| <span data-ttu-id="32999-156">Имя</span><span class="sxs-lookup"><span data-stu-id="32999-156">Name</span></span>       | <span data-ttu-id="32999-157">Тип</span><span class="sxs-lookup"><span data-stu-id="32999-157">Type</span></span> | <span data-ttu-id="32999-158">Описание</span><span class="sxs-lookup"><span data-stu-id="32999-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="32999-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="32999-159">Authorization</span></span>  | <span data-ttu-id="32999-160">string</span><span class="sxs-lookup"><span data-stu-id="32999-160">string</span></span>  | <span data-ttu-id="32999-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32999-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32999-163">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32999-163">Request body</span></span>

<span data-ttu-id="32999-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32999-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32999-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="32999-165">Response</span></span>

<span data-ttu-id="32999-166">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32999-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32999-167">Пример</span><span class="sxs-lookup"><span data-stu-id="32999-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="32999-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="32999-168">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="32999-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="32999-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="32999-170">C#</span><span class="sxs-lookup"><span data-stu-id="32999-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32999-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32999-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="32999-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="32999-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32999-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="32999-173">Response</span></span>

<span data-ttu-id="32999-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32999-174">Here is an example of the response.</span></span> <span data-ttu-id="32999-175">Note: ответ, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="32999-175">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="32999-176">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32999-176">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

<span data-ttu-id="32999-177">Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="32999-177">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="32999-178">Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="32999-178">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
