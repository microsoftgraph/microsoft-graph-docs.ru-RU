---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3ffcf78c7df28faba22b92a7389f473f0ea91613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335840"
---
# <a name="list-subscriptions"></a><span data-ttu-id="0cf5b-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="0cf5b-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cf5b-104">Получение списка подписок на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="0cf5b-105">Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf5b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf5b-106">Permissions</span></span>

<span data-ttu-id="0cf5b-107">Этот API поддерживает следующие области разрешений; Дополнительные сведения, в том числе выбор разрешений, приведены в разделе [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0cf5b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf5b-108">Permission type</span></span>  | <span data-ttu-id="0cf5b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cf5b-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="0cf5b-110">[Делегированный](/graph/auth-v2-user) (Рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cf5b-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="0cf5b-111">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="0cf5b-112">[Делегированный](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cf5b-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="0cf5b-113">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="0cf5b-114">Application</span><span class="sxs-lookup"><span data-stu-id="0cf5b-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="0cf5b-115">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="0cf5b-116">Результаты отКлика основываются на контексте вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="0cf5b-117">Ниже приведен краткий обзор типичных сценариев.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="0cf5b-118">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="0cf5b-118">Basic scenarios</span></span>

<span data-ttu-id="0cf5b-119">Чаще всего приложению требуется получить подписки, которые она создала для текущего пользователя, выполнившего вход в систему, или для всех пользователей в каталоге (рабочие и учебные учетные записи).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="0cf5b-120">Для этих сценариев не требуются специальные разрешения за пределами того приложения, которое использовалось изначально для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="0cf5b-121">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="0cf5b-121">Context of the calling app</span></span> | <span data-ttu-id="0cf5b-122">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="0cf5b-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="0cf5b-123">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="0cf5b-124">с</span><span class="sxs-lookup"><span data-stu-id="0cf5b-124">-and-</span></span><br/><span data-ttu-id="0cf5b-125">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="0cf5b-126">Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="0cf5b-127">Подписки, созданные **этим приложением** только для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="0cf5b-128">Приложение вызывается от имени самого себя (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="0cf5b-129">с</span><span class="sxs-lookup"><span data-stu-id="0cf5b-129">-and-</span></span><br/><span data-ttu-id="0cf5b-130">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="0cf5b-131">Примечание: это относится только к учетным записям рабочих и учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="0cf5b-132">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="0cf5b-133">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="0cf5b-133">Advanced scenarios</span></span>

<span data-ttu-id="0cf5b-134">В некоторых случаях приложению требуется получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="0cf5b-135">Например, пользователю необходимо просмотреть все подписки, созданные любым приложением от их имени.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="0cf5b-136">Кроме того, администратор может просмотреть все подписки на все приложения в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="0cf5b-137">В таких случаях необходимо делегировать подПиску с разрешениями. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="0cf5b-138">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="0cf5b-138">Context of the calling app</span></span> | <span data-ttu-id="0cf5b-139">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="0cf5b-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="0cf5b-140">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="0cf5b-141">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="0cf5b-142">с</span><span class="sxs-lookup"><span data-stu-id="0cf5b-142">-and-</span></span><br/><span data-ttu-id="0cf5b-143">Приложение имеет подПиску на разрешения. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0cf5b-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="0cf5b-144">Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="0cf5b-145">Подписки, созданные **любым приложением** только для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="0cf5b-146">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="0cf5b-147">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-147">*The user is an admin*.</span></span><br/><span data-ttu-id="0cf5b-148">с</span><span class="sxs-lookup"><span data-stu-id="0cf5b-148">-and-</span></span><br/><span data-ttu-id="0cf5b-149">Приложение имеет подПиску на разрешения. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0cf5b-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="0cf5b-150">Примечание: это относится только к учетным записям рабочих и учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="0cf5b-151">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cf5b-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cf5b-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cf5b-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0cf5b-153">Optional query parameters</span></span>

<span data-ttu-id="0cf5b-154">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cf5b-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cf5b-155">Request headers</span></span>

| <span data-ttu-id="0cf5b-156">Имя</span><span class="sxs-lookup"><span data-stu-id="0cf5b-156">Name</span></span>       | <span data-ttu-id="0cf5b-157">Тип</span><span class="sxs-lookup"><span data-stu-id="0cf5b-157">Type</span></span> | <span data-ttu-id="0cf5b-158">Описание</span><span class="sxs-lookup"><span data-stu-id="0cf5b-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0cf5b-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf5b-159">Authorization</span></span>  | <span data-ttu-id="0cf5b-160">string</span><span class="sxs-lookup"><span data-stu-id="0cf5b-160">string</span></span>  | <span data-ttu-id="0cf5b-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cf5b-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cf5b-163">Request body</span></span>

<span data-ttu-id="0cf5b-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cf5b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cf5b-165">Response</span></span>

<span data-ttu-id="0cf5b-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf5b-167">Пример</span><span class="sxs-lookup"><span data-stu-id="0cf5b-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0cf5b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cf5b-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="0cf5b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cf5b-169">Response</span></span>

<span data-ttu-id="0cf5b-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-170">Here is an example of the response.</span></span> <span data-ttu-id="0cf5b-171">Note: ответ, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="0cf5b-172">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-172">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->

<span data-ttu-id="0cf5b-173">Если запрос возвращает несколько страниц данных, ответ включает `@odata.nextLink` свойство, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="0cf5b-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="0cf5b-174">Дополнительные сведения см в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="0cf5b-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
