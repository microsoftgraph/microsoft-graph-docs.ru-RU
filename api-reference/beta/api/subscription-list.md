---
title: Перечисление подписок
description: " в приведенных ниже сценариях представлены подробные сведения."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537092"
---
# <a name="list-subscriptions"></a><span data-ttu-id="80038-103">Перечисление подписок</span><span class="sxs-lookup"><span data-stu-id="80038-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80038-104">Получение списка подписок на веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="80038-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="80038-105">Содержимое ответа зависит от контекста, в котором приложение вызывается; в приведенных ниже сценариях представлены подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="80038-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="80038-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80038-106">Permissions</span></span>

<span data-ttu-id="80038-107">Этот API поддерживает следующие области разрешений; Дополнительные сведения, в том числе выбор разрешений, приведены в разделе [разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80038-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80038-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80038-108">Permission type</span></span>  | <span data-ttu-id="80038-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80038-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="80038-110">[Делегированный](/graph/auth-v2-user) (Рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80038-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="80038-111">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="80038-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="80038-112">[Делегированный](/graph/auth-v2-user) (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80038-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="80038-113">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md) или подписки. Read. All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="80038-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="80038-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="80038-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="80038-115">Разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="80038-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="80038-116">Результаты отКлика основываются на контексте вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="80038-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="80038-117">Ниже приведен краткий обзор типичных сценариев.</span><span class="sxs-lookup"><span data-stu-id="80038-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="80038-118">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="80038-118">Basic scenarios</span></span>

<span data-ttu-id="80038-119">Чаще всего приложению требуется получить подписки, которые она создала для текущего пользователя, выполнившего вход в систему, или для всех пользователей в каталоге (рабочие и учебные учетные записи).</span><span class="sxs-lookup"><span data-stu-id="80038-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="80038-120">Для этих сценариев не требуются специальные разрешения за пределами того приложения, которое использовалось изначально для создания своих подписок.</span><span class="sxs-lookup"><span data-stu-id="80038-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="80038-121">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="80038-121">Context of the calling app</span></span> | <span data-ttu-id="80038-122">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="80038-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="80038-123">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="80038-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="80038-124">с</span><span class="sxs-lookup"><span data-stu-id="80038-124">-and-</span></span><br/><span data-ttu-id="80038-125">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="80038-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="80038-126">Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="80038-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="80038-127">Подписки, созданные **этим приложением** только для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="80038-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="80038-128">Приложение вызывается от имени самого себя (разрешение приложения).</span><span class="sxs-lookup"><span data-stu-id="80038-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="80038-129">с</span><span class="sxs-lookup"><span data-stu-id="80038-129">-and-</span></span><br/><span data-ttu-id="80038-130">У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="80038-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="80038-131">Примечание: это относится только к учетным записям рабочих и учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="80038-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="80038-132">Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="80038-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="80038-133">Расширенные сценарии</span><span class="sxs-lookup"><span data-stu-id="80038-133">Advanced scenarios</span></span>

<span data-ttu-id="80038-134">В некоторых случаях приложению требуется получить подписки, созданные другими приложениями.</span><span class="sxs-lookup"><span data-stu-id="80038-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="80038-135">Например, пользователю необходимо просмотреть все подписки, созданные любым приложением от их имени.</span><span class="sxs-lookup"><span data-stu-id="80038-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="80038-136">Кроме того, администратор может просмотреть все подписки на все приложения в своем каталоге.</span><span class="sxs-lookup"><span data-stu-id="80038-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="80038-137">В таких случаях необходимо делегировать подПиску с разрешениями. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="80038-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="80038-138">Контекст вызывающего приложения</span><span class="sxs-lookup"><span data-stu-id="80038-138">Context of the calling app</span></span> | <span data-ttu-id="80038-139">Ответ содержит</span><span class="sxs-lookup"><span data-stu-id="80038-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="80038-140">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="80038-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="80038-141">*Пользователь не является администратором*.</span><span class="sxs-lookup"><span data-stu-id="80038-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="80038-142">с</span><span class="sxs-lookup"><span data-stu-id="80038-142">-and-</span></span><br/><span data-ttu-id="80038-143">Приложение имеет подПиску на разрешения. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="80038-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="80038-144">Примечание: это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="80038-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="80038-145">Подписки, созданные **любым приложением** только для пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="80038-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="80038-146">Приложение звонит от имени пользователя, выполнившего вход в систему (делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="80038-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="80038-147">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="80038-147">*The user is an admin*.</span></span><br/><span data-ttu-id="80038-148">с</span><span class="sxs-lookup"><span data-stu-id="80038-148">-and-</span></span><br/><span data-ttu-id="80038-149">Приложение имеет подПиску на разрешения. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="80038-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="80038-150">Примечание: это относится только к учетным записям рабочих и учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="80038-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="80038-151">Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="80038-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80038-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80038-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80038-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="80038-153">Optional query parameters</span></span>

<span data-ttu-id="80038-154">Этот метод не поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="80038-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80038-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80038-155">Request headers</span></span>

| <span data-ttu-id="80038-156">Имя</span><span class="sxs-lookup"><span data-stu-id="80038-156">Name</span></span>       | <span data-ttu-id="80038-157">Тип</span><span class="sxs-lookup"><span data-stu-id="80038-157">Type</span></span> | <span data-ttu-id="80038-158">Описание</span><span class="sxs-lookup"><span data-stu-id="80038-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80038-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="80038-159">Authorization</span></span>  | <span data-ttu-id="80038-160">string</span><span class="sxs-lookup"><span data-stu-id="80038-160">string</span></span>  | <span data-ttu-id="80038-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80038-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80038-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80038-163">Request body</span></span>

<span data-ttu-id="80038-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80038-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80038-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="80038-165">Response</span></span>

<span data-ttu-id="80038-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список объектов [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80038-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80038-167">Пример</span><span class="sxs-lookup"><span data-stu-id="80038-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80038-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="80038-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="80038-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="80038-169">Response</span></span>

<span data-ttu-id="80038-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="80038-170">Here is an example of the response.</span></span> <span data-ttu-id="80038-171">Note: ответ, показанный здесь, может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="80038-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="80038-172">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80038-172">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<span data-ttu-id="80038-173">Если запрос возвращает несколько страниц данных, ответ включает `@odata.nextLink` свойство, помогающее управлять результатами.</span><span class="sxs-lookup"><span data-stu-id="80038-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="80038-174">Дополнительные сведения см в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="80038-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
