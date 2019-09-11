---
title: 'вызов: отклонено'
description: Отклонение входящего вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e3befe394aa9451cbb51bd39ba41fb158b67b464
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838848"
---
# <a name="call-reject"></a><span data-ttu-id="8a03e-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="8a03e-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a03e-104">Позволяет роботу отклонить входящий [вызов](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="8a03e-104">Enables the bot to reject an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="8a03e-105">Запрос входящего вызова может представлять собой приглашение на собрание или одноранговый вызов.</span><span class="sxs-lookup"><span data-stu-id="8a03e-105">The incoming call request can be an invite to a meeting or a peer to peer call.</span></span> <span data-ttu-id="8a03e-106">Время ожидания входящего вызова истекает через 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="8a03e-106">The incoming call request times out after 15 seconds.</span></span> <span data-ttu-id="8a03e-107">Если в течение этого времени отклики не отправляются, вызов автоматически отклоняется.</span><span class="sxs-lookup"><span data-stu-id="8a03e-107">If no response is sent during this time, the call is automatically rejected.</span></span>

<span data-ttu-id="8a03e-108">После регистрации Bot с действительным URL-адресом обратного вызова на портале Azure входящий вызов доставляется [](../resources/commsnotification.md) в качестве `changeType` коммснотификатион со `created`значением.</span><span class="sxs-lookup"><span data-stu-id="8a03e-108">Once the bot is registered with a valid callback URL in the Azure portal, the incoming call is delivered as a [commsNotification](../resources/commsnotification.md) with `changeType` set to `created`.</span></span> <span data-ttu-id="8a03e-109">Ожидается, что для `Answer` начала и `Reject` до истечения времени ожидания вызывается Bot.</span><span class="sxs-lookup"><span data-stu-id="8a03e-109">The bot is expected to `Answer` or `Reject` the call before it times out.</span></span>

> <span data-ttu-id="8a03e-110">**Примечание:** Этот API используется только для отклонения входящих вызовов.</span><span class="sxs-lookup"><span data-stu-id="8a03e-110">**Note:** This API is only used to reject incoming calls.</span></span> <span data-ttu-id="8a03e-111">Для прерывания существующих вызовов вместо этого следует использовать [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="8a03e-111">To terminate existing calls, [Delete Call](../api/call-delete.md) should be used instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a03e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a03e-112">Permissions</span></span>
<span data-ttu-id="8a03e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a03e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8a03e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a03e-115">Permission type</span></span> | <span data-ttu-id="8a03e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a03e-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8a03e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a03e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="8a03e-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8a03e-118">Not Supported</span></span>                       |
| <span data-ttu-id="8a03e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a03e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a03e-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8a03e-120">Not Supported</span></span>                       |
| <span data-ttu-id="8a03e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a03e-121">Application</span></span>     | <span data-ttu-id="8a03e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8a03e-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="8a03e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a03e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="8a03e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a03e-124">Request headers</span></span>
| <span data-ttu-id="8a03e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="8a03e-125">Name</span></span>          | <span data-ttu-id="8a03e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8a03e-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8a03e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a03e-127">Authorization</span></span> | <span data-ttu-id="8a03e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a03e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a03e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a03e-130">Request body</span></span>
<span data-ttu-id="8a03e-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8a03e-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a03e-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="8a03e-132">Parameter</span></span>      | <span data-ttu-id="8a03e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8a03e-133">Type</span></span>    |<span data-ttu-id="8a03e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8a03e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a03e-135">причиной</span><span class="sxs-lookup"><span data-stu-id="8a03e-135">reason</span></span>|<span data-ttu-id="8a03e-136">String.</span><span class="sxs-lookup"><span data-stu-id="8a03e-136">String</span></span>|<span data-ttu-id="8a03e-137">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="8a03e-137">The rejection reason.</span></span> <span data-ttu-id="8a03e-138">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="8a03e-138">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="8a03e-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="8a03e-139">callbackUri</span></span>|<span data-ttu-id="8a03e-140">String</span><span class="sxs-lookup"><span data-stu-id="8a03e-140">String</span></span>|<span data-ttu-id="8a03e-141">Позволяет Боты предоставить определенный URI обратного вызова, в котором будет опубликован результат действия "отклонить".</span><span class="sxs-lookup"><span data-stu-id="8a03e-141">Allows bots to provide a specific callback URI where the result of the Reject action will be posted.</span></span> <span data-ttu-id="8a03e-142">Это позволяет отправить результат в тот же конкретный экземпляр ленты, который инициировал действие отклонения.</span><span class="sxs-lookup"><span data-stu-id="8a03e-142">This allows sending the result to the same specific bot instance that triggered the Reject action.</span></span> <span data-ttu-id="8a03e-143">Если он не указан, будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="8a03e-143">If none is provided, the bot's global callback URI will be used.</span></span>|

## <a name="response"></a><span data-ttu-id="8a03e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a03e-144">Response</span></span>
<span data-ttu-id="8a03e-p108">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8a03e-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8a03e-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="8a03e-147">Examples</span></span>
<span data-ttu-id="8a03e-148">В приведенных ниже примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8a03e-148">The following examples shows how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="8a03e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a03e-149">Request</span></span>
<span data-ttu-id="8a03e-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a03e-150">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a03e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a03e-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a03e-152">C#</span><span class="sxs-lookup"><span data-stu-id="8a03e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a03e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a03e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a03e-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8a03e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="8a03e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a03e-155">Response</span></span>
<span data-ttu-id="8a03e-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a03e-156">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="8a03e-157">Отклонение входящего звонка с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="8a03e-157">Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="8a03e-158">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="8a03e-158">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="8a03e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a03e-159">Request</span></span>
<span data-ttu-id="8a03e-160">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a03e-160">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a03e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a03e-161">HTTP</span></span>](#tab/http)

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a03e-162">C#</span><span class="sxs-lookup"><span data-stu-id="8a03e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a03e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a03e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a03e-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8a03e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8a03e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a03e-165">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="8a03e-166">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="8a03e-166">Notification - deleted</span></span>

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
