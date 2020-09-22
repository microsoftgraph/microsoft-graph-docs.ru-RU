---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a9164b90d8b3156fa9abb57d41767c9a322f7c27
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193451"
---
# <a name="list-subscriptions"></a><span data-ttu-id="71edb-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="71edb-103">List subscriptions</span></span>

<span data-ttu-id="71edb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71edb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71edb-105">Получение списка подписок на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="71edb-105">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="71edb-106">Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="71edb-106">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="71edb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71edb-107">Permissions</span></span>

<span data-ttu-id="71edb-108">Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71edb-108">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71edb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71edb-109">Permission type</span></span>  | <span data-ttu-id="71edb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71edb-110">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="71edb-111">[Делегированная](/graph/auth-v2-user) (Рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71edb-111">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="71edb-112">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="71edb-112">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="71edb-113">[Делегированная](/graph/auth-v2-user) учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71edb-113">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="71edb-114">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="71edb-114">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="71edb-115">Application</span><span class="sxs-lookup"><span data-stu-id="71edb-115">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="71edb-116">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="71edb-116">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="71edb-117">Результаты отклика основаны на контексте приложения, отправившего вызов.</span><span class="sxs-lookup"><span data-stu-id="71edb-117">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="71edb-118">Ниже представлена сводка общих сценариев.</span><span class="sxs-lookup"><span data-stu-id="71edb-118">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="71edb-119">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="71edb-119">Basic scenarios</span></span>

<span data-ttu-id="71edb-120">Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей).</span><span class="sxs-lookup"><span data-stu-id="71edb-120">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="71edb-121">В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="71edb-121">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="71edb-122">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="71edb-122">Context of the calling app</span></span> | <span data-ttu-id="71edb-123">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="71edb-123">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="71edb-124">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="71edb-124">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="71edb-125">-и-</span><span class="sxs-lookup"><span data-stu-id="71edb-125">-and-</span></span><br/><span data-ttu-id="71edb-126">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="71edb-126">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="71edb-127">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="71edb-127">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="71edb-128">Подписки, созданные **этим приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="71edb-128">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="71edb-129">Приложение отправляет вызов от своего имени (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="71edb-129">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="71edb-130">-и-</span><span class="sxs-lookup"><span data-stu-id="71edb-130">-and-</span></span><br/><span data-ttu-id="71edb-131">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="71edb-131">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="71edb-132">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="71edb-132">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="71edb-133">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="71edb-133">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="71edb-134">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="71edb-134">Advanced scenarios</span></span>

<span data-ttu-id="71edb-135">В некоторых случаях приложению нужно получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="71edb-135">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="71edb-136">Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени.</span><span class="sxs-lookup"><span data-stu-id="71edb-136">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="71edb-137">Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="71edb-137">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="71edb-138">В таких сценариях требуется делегированное разрешение Subscription.Read.All.</span><span class="sxs-lookup"><span data-stu-id="71edb-138">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="71edb-139">Контекст приложения, отправившего вызов</span><span class="sxs-lookup"><span data-stu-id="71edb-139">Context of the calling app</span></span> | <span data-ttu-id="71edb-140">Состав отклика</span><span class="sxs-lookup"><span data-stu-id="71edb-140">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="71edb-141">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="71edb-141">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="71edb-142">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="71edb-142">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="71edb-143">-и-</span><span class="sxs-lookup"><span data-stu-id="71edb-143">-and-</span></span><br/><span data-ttu-id="71edb-144">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="71edb-144">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="71edb-145">Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="71edb-145">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="71edb-146">Подписки, созданные **любым приложением** только для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="71edb-146">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="71edb-147">Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="71edb-147">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="71edb-148">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="71edb-148">*The user is an admin*.</span></span><br/><span data-ttu-id="71edb-149">-и-</span><span class="sxs-lookup"><span data-stu-id="71edb-149">-and-</span></span><br/><span data-ttu-id="71edb-150">У приложения есть разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="71edb-150">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="71edb-151">Примечание. Это относится только к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="71edb-151">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="71edb-152">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="71edb-152">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71edb-153">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71edb-153">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71edb-154">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71edb-154">Optional query parameters</span></span>

<span data-ttu-id="71edb-155">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="71edb-155">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71edb-156">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71edb-156">Request headers</span></span>

| <span data-ttu-id="71edb-157">Имя</span><span class="sxs-lookup"><span data-stu-id="71edb-157">Name</span></span>       | <span data-ttu-id="71edb-158">Тип</span><span class="sxs-lookup"><span data-stu-id="71edb-158">Type</span></span> | <span data-ttu-id="71edb-159">Описание</span><span class="sxs-lookup"><span data-stu-id="71edb-159">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71edb-160">Authorization</span><span class="sxs-lookup"><span data-stu-id="71edb-160">Authorization</span></span>  | <span data-ttu-id="71edb-161">string</span><span class="sxs-lookup"><span data-stu-id="71edb-161">string</span></span>  | <span data-ttu-id="71edb-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71edb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71edb-164">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71edb-164">Request body</span></span>

<span data-ttu-id="71edb-165">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71edb-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71edb-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="71edb-166">Response</span></span>

<span data-ttu-id="71edb-167">В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71edb-167">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71edb-168">Пример</span><span class="sxs-lookup"><span data-stu-id="71edb-168">Example</span></span>

##### <a name="request"></a><span data-ttu-id="71edb-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="71edb-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="71edb-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="71edb-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[<span data-ttu-id="71edb-171">C#</span><span class="sxs-lookup"><span data-stu-id="71edb-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71edb-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71edb-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71edb-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71edb-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71edb-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="71edb-174">Response</span></span>

<span data-ttu-id="71edb-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71edb-175">Here is an example of the response.</span></span> <span data-ttu-id="71edb-176">Note: ответ, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="71edb-176">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="71edb-177">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71edb-177">All of the properties will be returned from an actual call.</span></span>

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
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false
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

> <span data-ttu-id="71edb-178">**Примечание.** Значение свойства `clientState` не возвращается в целях безопасности.</span><span class="sxs-lookup"><span data-stu-id="71edb-178">**Note:** the `clientState` property value is not returned for security purposes.</span></span>  

<span data-ttu-id="71edb-179">Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="71edb-179">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="71edb-180">Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="71edb-180">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>


