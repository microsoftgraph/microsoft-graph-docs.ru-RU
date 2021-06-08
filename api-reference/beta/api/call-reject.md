---
title: 'вызов: отклонить'
description: Включить бот, чтобы отклонить входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e734ae62b669b178b81fcb0f63db96d734591d9f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786568"
---
# <a name="call-reject"></a><span data-ttu-id="fd8df-103">вызов: отклонить</span><span class="sxs-lookup"><span data-stu-id="fd8df-103">call: reject</span></span>

<span data-ttu-id="fd8df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd8df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd8df-105">Включить бот, чтобы отклонить входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="fd8df-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="fd8df-106">Входящий запрос может быть приглашением от участника группового звонка или одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="fd8df-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="fd8df-107">Если приглашение на групповой вызов получено, уведомление будет содержать **параметры chatInfo** и **meetingInfo.**</span><span class="sxs-lookup"><span data-stu-id="fd8df-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="fd8df-108">Ожидается, что бот ответит или отклоняет вызов до времени вызова. Текущее значение времени времени — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="fd8df-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="fd8df-109">Этот API не заканчивает существующие вызовы, которые уже ответили.</span><span class="sxs-lookup"><span data-stu-id="fd8df-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="fd8df-110">Чтобы [закончить](../api/call-delete.md) вызов, используйте вызов удаления.</span><span class="sxs-lookup"><span data-stu-id="fd8df-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd8df-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd8df-111">Permissions</span></span>
<span data-ttu-id="fd8df-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd8df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd8df-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd8df-114">Permission type</span></span> | <span data-ttu-id="fd8df-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd8df-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="fd8df-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd8df-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd8df-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd8df-117">Not Supported</span></span>                       |
| <span data-ttu-id="fd8df-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd8df-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd8df-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="fd8df-119">Not Supported</span></span>                       |
| <span data-ttu-id="fd8df-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="fd8df-120">Application</span></span>     | <span data-ttu-id="fd8df-121">Нет</span><span class="sxs-lookup"><span data-stu-id="fd8df-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="fd8df-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd8df-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="fd8df-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="fd8df-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="fd8df-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="fd8df-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd8df-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd8df-125">Request headers</span></span>
| <span data-ttu-id="fd8df-126">Имя</span><span class="sxs-lookup"><span data-stu-id="fd8df-126">Name</span></span>          | <span data-ttu-id="fd8df-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fd8df-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fd8df-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd8df-128">Authorization</span></span> | <span data-ttu-id="fd8df-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd8df-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd8df-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd8df-131">Content-type</span></span>  | <span data-ttu-id="fd8df-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd8df-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd8df-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd8df-134">Request body</span></span>
<span data-ttu-id="fd8df-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fd8df-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fd8df-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="fd8df-136">Parameter</span></span>      | <span data-ttu-id="fd8df-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fd8df-137">Type</span></span>    |<span data-ttu-id="fd8df-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fd8df-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd8df-139">reason</span><span class="sxs-lookup"><span data-stu-id="fd8df-139">reason</span></span>|<span data-ttu-id="fd8df-140">String</span><span class="sxs-lookup"><span data-stu-id="fd8df-140">String</span></span>|<span data-ttu-id="fd8df-141">Причина отказа.</span><span class="sxs-lookup"><span data-stu-id="fd8df-141">The rejection reason.</span></span> <span data-ttu-id="fd8df-142">Возможные значения: `None` и `Busy``Forbidden`</span><span class="sxs-lookup"><span data-stu-id="fd8df-142">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="fd8df-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="fd8df-143">callbackUri</span></span>|<span data-ttu-id="fd8df-144">String</span><span class="sxs-lookup"><span data-stu-id="fd8df-144">String</span></span>|<span data-ttu-id="fd8df-145">Это позволяет ботам предоставлять определенный URI вызова для текущего вызова для получения более поздних уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fd8df-145">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="fd8df-146">Если это свойство не установлено, вместо него будет использоваться глобальный URI вызова бота.</span><span class="sxs-lookup"><span data-stu-id="fd8df-146">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="fd8df-147">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="fd8df-147">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="fd8df-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd8df-148">Response</span></span>
<span data-ttu-id="fd8df-p109">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd8df-p109">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd8df-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd8df-151">Examples</span></span>
<span data-ttu-id="fd8df-152">В следующих примерах покажите, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="fd8df-152">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="fd8df-153">Пример 1. Отклонение входящих вызовов по причине "занят"</span><span class="sxs-lookup"><span data-stu-id="fd8df-153">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="fd8df-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd8df-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fd8df-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd8df-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="c"></a>[<span data-ttu-id="fd8df-156">C#</span><span class="sxs-lookup"><span data-stu-id="fd8df-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="fd8df-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd8df-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="fd8df-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd8df-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="java"></a>[<span data-ttu-id="fd8df-159">Java</span><span class="sxs-lookup"><span data-stu-id="fd8df-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="fd8df-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd8df-160">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="fd8df-161">Пример 2. Отклонение входящих вызовов по причине "Нет"</span><span class="sxs-lookup"><span data-stu-id="fd8df-161">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="fd8df-162">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="fd8df-162">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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

##### <a name="request"></a><span data-ttu-id="fd8df-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd8df-163">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fd8df-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd8df-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="c"></a>[<span data-ttu-id="fd8df-165">C#</span><span class="sxs-lookup"><span data-stu-id="fd8df-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd8df-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd8df-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd8df-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd8df-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd8df-168">Java</span><span class="sxs-lookup"><span data-stu-id="fd8df-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fd8df-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd8df-169">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="fd8df-170">Уведомление — удалено</span><span class="sxs-lookup"><span data-stu-id="fd8df-170">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896"
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


