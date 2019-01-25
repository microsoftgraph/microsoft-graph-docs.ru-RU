---
title: Список подписок
description: " сценарии ниже для получения дополнительных сведений см."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510983"
---
# <a name="list-subscriptions"></a><span data-ttu-id="a453b-103">Список подписок</span><span class="sxs-lookup"><span data-stu-id="a453b-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a453b-104">Получение списка webhook подписки.</span><span class="sxs-lookup"><span data-stu-id="a453b-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="a453b-105">Содержимое ответа зависит от контекста, в котором вызов приложения; сценарии ниже для получения дополнительных сведений см.</span><span class="sxs-lookup"><span data-stu-id="a453b-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a453b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a453b-106">Permissions</span></span>

<span data-ttu-id="a453b-107">Этот интерфейс API поддерживает следующие области разрешений; [для получения дополнительных сведений, включая выбор разрешений, см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="a453b-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a453b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a453b-108">Permission type</span></span>  | <span data-ttu-id="a453b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a453b-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="a453b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a453b-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="a453b-111">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="a453b-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="a453b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a453b-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="a453b-113">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md) или Subscription.Read.All (см. ниже).</span><span class="sxs-lookup"><span data-stu-id="a453b-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="a453b-114">Application</span><span class="sxs-lookup"><span data-stu-id="a453b-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="a453b-115">Разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a453b-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="a453b-116">Результаты ответа зависят от контекста вызова приложения.</span><span class="sxs-lookup"><span data-stu-id="a453b-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="a453b-117">Ниже приведен перечень распространенных сценариев:</span><span class="sxs-lookup"><span data-stu-id="a453b-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="a453b-118">Основные сценарии</span><span class="sxs-lookup"><span data-stu-id="a453b-118">Basic scenarios</span></span>

<span data-ttu-id="a453b-119">Чаще всего приложения, где требуется реализовать для получения подписки, для которых он создан для пользователя, вошедшего в систему, или для всех пользователей в каталоге (рабочего/школа учетные записи).</span><span class="sxs-lookup"><span data-stu-id="a453b-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="a453b-120">Эти сценарии не требуются любые специальные разрешения, помимо тех, которые соответствуют приложения, изначально используется для создания его подписки.</span><span class="sxs-lookup"><span data-stu-id="a453b-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="a453b-121">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="a453b-121">Context of the calling app</span></span> | <span data-ttu-id="a453b-122">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="a453b-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="a453b-123">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a453b-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="a453b-124">And</span><span class="sxs-lookup"><span data-stu-id="a453b-124">-and-</span></span><br/><span data-ttu-id="a453b-125">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a453b-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="a453b-126">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a453b-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="a453b-127">Подписки, созданные **в этом приложении** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a453b-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="a453b-128">Приложение вызов от имени самого (разрешений приложения).</span><span class="sxs-lookup"><span data-stu-id="a453b-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="a453b-129">And</span><span class="sxs-lookup"><span data-stu-id="a453b-129">-and-</span></span><br/><span data-ttu-id="a453b-130">Приложение обладает исходного разрешения, необходимые для [создания подписки](subscription-post-subscriptions.md).</span><span class="sxs-lookup"><span data-stu-id="a453b-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="a453b-131">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a453b-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="a453b-132">Подписки, созданные **в этом приложении** для себя или для любого пользователя в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a453b-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="a453b-133">Дополнительные сценарии</span><span class="sxs-lookup"><span data-stu-id="a453b-133">Advanced scenarios</span></span>

<span data-ttu-id="a453b-134">В некоторых случаях приложения, где требуется реализовать для получения подписки, созданные в других приложениях.</span><span class="sxs-lookup"><span data-stu-id="a453b-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="a453b-135">Например пользователю для просмотра всех подписок, созданных любого приложения от их имени.</span><span class="sxs-lookup"><span data-stu-id="a453b-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="a453b-136">Или администратор может потребоваться просмотреть все подписки из всех приложений в своих каталогов.</span><span class="sxs-lookup"><span data-stu-id="a453b-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="a453b-137">Для таких сценариев делегированных разрешений Subscription.Read.All является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a453b-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="a453b-138">Контекст приложения, вызывающего</span><span class="sxs-lookup"><span data-stu-id="a453b-138">Context of the calling app</span></span> | <span data-ttu-id="a453b-139">Содержит ответа</span><span class="sxs-lookup"><span data-stu-id="a453b-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="a453b-140">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a453b-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="a453b-141">*Пользователь является без прав администратора*.</span><span class="sxs-lookup"><span data-stu-id="a453b-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="a453b-142">And</span><span class="sxs-lookup"><span data-stu-id="a453b-142">-and-</span></span><br/><span data-ttu-id="a453b-143">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="a453b-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="a453b-144">Примечание: Это относится к личных учетных записей Майкрософт и работы/школа учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a453b-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="a453b-145">Подписки, созданные в **любое приложение** выполнил вход только для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a453b-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="a453b-146">Приложение вызов от имени выполнившего вход пользователя (делегированных разрешений).</span><span class="sxs-lookup"><span data-stu-id="a453b-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="a453b-147">*Пользователь является администратором*.</span><span class="sxs-lookup"><span data-stu-id="a453b-147">*The user is an admin*.</span></span><br/><span data-ttu-id="a453b-148">And</span><span class="sxs-lookup"><span data-stu-id="a453b-148">-and-</span></span><br/><span data-ttu-id="a453b-149">Приложение имеет разрешение Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="a453b-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="a453b-150">Примечание: Это относится к рабочих/школа только для учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a453b-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="a453b-151">Подписки, созданные с **любого приложения** для **любого пользователя** в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a453b-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a453b-152">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a453b-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a453b-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a453b-153">Optional query parameters</span></span>

<span data-ttu-id="a453b-154">Этот метод не поддерживает [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="a453b-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a453b-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a453b-155">Request headers</span></span>

| <span data-ttu-id="a453b-156">Имя</span><span class="sxs-lookup"><span data-stu-id="a453b-156">Name</span></span>       | <span data-ttu-id="a453b-157">Тип</span><span class="sxs-lookup"><span data-stu-id="a453b-157">Type</span></span> | <span data-ttu-id="a453b-158">Описание</span><span class="sxs-lookup"><span data-stu-id="a453b-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a453b-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="a453b-159">Authorization</span></span>  | <span data-ttu-id="a453b-160">string</span><span class="sxs-lookup"><span data-stu-id="a453b-160">string</span></span>  | <span data-ttu-id="a453b-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a453b-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a453b-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a453b-163">Request body</span></span>

<span data-ttu-id="a453b-164">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a453b-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a453b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="a453b-165">Response</span></span>

<span data-ttu-id="a453b-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и список объектов [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a453b-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a453b-167">Пример</span><span class="sxs-lookup"><span data-stu-id="a453b-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a453b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="a453b-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="a453b-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="a453b-169">Response</span></span>

<span data-ttu-id="a453b-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a453b-170">Here is an example of the response.</span></span> <span data-ttu-id="a453b-171">Примечание: Для краткости может усекаться ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="a453b-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="a453b-172">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a453b-172">All of the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="a453b-173">При возврате нескольких страниц данных ответа включает в себя `@odata.nextLink` свойство, чтобы помочь вам управлять результаты.</span><span class="sxs-lookup"><span data-stu-id="a453b-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="a453b-174">Для получения дополнительных сведений см [Microsoft Graph постраничного просмотра данных в вашем приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="a453b-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
