---
title: 'вызов: отклонено'
description: Отклонение входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0134b03e27deeaf24eba3deb9c58b56865ab72d8
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792285"
---
# <a name="call-reject"></a><span data-ttu-id="c1095-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="c1095-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1095-104">Позволяет роботу отклонить входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="c1095-104">Enables the bot to reject an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="c1095-105">Запрос входящего вызова может представлять собой приглашение на собрание или одноранговый вызов.</span><span class="sxs-lookup"><span data-stu-id="c1095-105">The incoming call request can be an invite to a meeting or a peer to peer call.</span></span> <span data-ttu-id="c1095-106">Время ожидания входящего вызова истекает через 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="c1095-106">The incoming call request times out after 15 seconds.</span></span> <span data-ttu-id="c1095-107">Если в течение этого времени отклики не отправляются, вызов автоматически отклоняется.</span><span class="sxs-lookup"><span data-stu-id="c1095-107">If no response is sent during this time, the call is automatically rejected.</span></span>

<span data-ttu-id="c1095-108">После регистрации Bot с действительным URL-адресом обратного вызова на портале Azure входящий вызов доставляется [](../resources/commsnotification.md) в качестве `changeType` коммснотификатион со `created`значением.</span><span class="sxs-lookup"><span data-stu-id="c1095-108">Once the bot is registered with a valid callback URL in the Azure portal, the incoming call is delivered as a [commsNotification](../resources/commsnotification.md) with `changeType` set to `created`.</span></span> <span data-ttu-id="c1095-109">Ожидается, что для `Answer` начала и `Reject` до истечения времени ожидания вызывается Bot.</span><span class="sxs-lookup"><span data-stu-id="c1095-109">The bot is expected to `Answer` or `Reject` the call before it times out.</span></span>

> <span data-ttu-id="c1095-110">**Примечание:** Этот API используется только для отклонения входящих вызовов.</span><span class="sxs-lookup"><span data-stu-id="c1095-110">**Note:** This API is only used to reject incoming calls.</span></span> <span data-ttu-id="c1095-111">Для прерывания существующих вызовов вместо этого следует использовать [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="c1095-111">To terminate existing calls, [Delete Call](../api/call-delete.md) should be used instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1095-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1095-112">Permissions</span></span>
<span data-ttu-id="c1095-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1095-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1095-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1095-115">Permission type</span></span> | <span data-ttu-id="c1095-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1095-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="c1095-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1095-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1095-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c1095-118">Not Supported</span></span>                       |
| <span data-ttu-id="c1095-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1095-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1095-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c1095-120">Not Supported</span></span>                       |
| <span data-ttu-id="c1095-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1095-121">Application</span></span>     | <span data-ttu-id="c1095-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c1095-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="c1095-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1095-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="c1095-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1095-124">Request headers</span></span>
| <span data-ttu-id="c1095-125">Имя</span><span class="sxs-lookup"><span data-stu-id="c1095-125">Name</span></span>          | <span data-ttu-id="c1095-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c1095-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c1095-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1095-127">Authorization</span></span> | <span data-ttu-id="c1095-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1095-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1095-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1095-130">Request body</span></span>
<span data-ttu-id="c1095-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c1095-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1095-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1095-132">Parameter</span></span>      | <span data-ttu-id="c1095-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c1095-133">Type</span></span>    |<span data-ttu-id="c1095-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c1095-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1095-135">причиной</span><span class="sxs-lookup"><span data-stu-id="c1095-135">reason</span></span>|<span data-ttu-id="c1095-136">String.</span><span class="sxs-lookup"><span data-stu-id="c1095-136">String</span></span>|<span data-ttu-id="c1095-137">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="c1095-137">The rejection reason.</span></span> <span data-ttu-id="c1095-138">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="c1095-138">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="c1095-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="c1095-139">callbackUri</span></span>|<span data-ttu-id="c1095-140">String</span><span class="sxs-lookup"><span data-stu-id="c1095-140">String</span></span>|<span data-ttu-id="c1095-141">Позволяет Боты предоставить определенный URI обратного вызова, в котором будет опубликован результат действия "отклонить".</span><span class="sxs-lookup"><span data-stu-id="c1095-141">Allows bots to provide a specific callback URI where the result of the Reject action will be posted.</span></span> <span data-ttu-id="c1095-142">Это позволяет отправить результат в тот же конкретный экземпляр ленты, который инициировал действие отклонения.</span><span class="sxs-lookup"><span data-stu-id="c1095-142">This allows sending the result to the same specific bot instance that triggered the Reject action.</span></span> <span data-ttu-id="c1095-143">Если он не указан, будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="c1095-143">If none is provided, the bot's global callback URI will be used.</span></span>|

## <a name="response"></a><span data-ttu-id="c1095-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1095-144">Response</span></span>
<span data-ttu-id="c1095-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c1095-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1095-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1095-147">Examples</span></span>
<span data-ttu-id="c1095-148">В приведенных ниже примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c1095-148">The following examples shows how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="c1095-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1095-149">Request</span></span>
<span data-ttu-id="c1095-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1095-150">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1095-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1095-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1095-152">C#</span><span class="sxs-lookup"><span data-stu-id="c1095-152">C#</span></span>](#tab/csharp) 
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1095-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1095-153">Javascript</span></span>](#tab/javascript) 
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1095-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1095-154">Objective-C</span></span>](#tab/objc)  
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]    
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="c1095-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1095-155">Response</span></span>
<span data-ttu-id="c1095-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1095-156">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="c1095-157">Отклонение входящего звонка с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="c1095-157">Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="c1095-158">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="c1095-158">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "John",
              "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="c1095-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1095-159">Request</span></span>
<span data-ttu-id="c1095-160">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1095-160">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1095-161">C#</span><span class="sxs-lookup"><span data-stu-id="c1095-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1095-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1095-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1095-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c1095-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1095-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1095-164">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="c1095-165">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="c1095-165">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
