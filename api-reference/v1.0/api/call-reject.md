---
title: 'вызов: отклонить'
description: Включить бот, чтобы отклонить входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1355a826ab3bfaeea3392e20a6e40c71a279ca58
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787494"
---
# <a name="call-reject"></a><span data-ttu-id="e3c42-103">вызов: отклонить</span><span class="sxs-lookup"><span data-stu-id="e3c42-103">call: reject</span></span>

<span data-ttu-id="e3c42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3c42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3c42-105">Включить бот, чтобы отклонить входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="e3c42-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="e3c42-106">Входящий запрос может быть приглашением от участника группового звонка или одноранговых вызовов.</span><span class="sxs-lookup"><span data-stu-id="e3c42-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="e3c42-107">Если приглашение на групповой вызов получено, уведомление будет содержать **параметры chatInfo** и **meetingInfo.**</span><span class="sxs-lookup"><span data-stu-id="e3c42-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="e3c42-108">Ожидается, что бот ответит или отклоняет вызов до времени вызова. Текущее значение времени времени — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="e3c42-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="e3c42-109">Этот API не заканчивает существующие вызовы, которые уже ответили.</span><span class="sxs-lookup"><span data-stu-id="e3c42-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="e3c42-110">Чтобы [закончить](../api/call-delete.md) вызов, используйте вызов удаления.</span><span class="sxs-lookup"><span data-stu-id="e3c42-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3c42-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3c42-111">Permissions</span></span>
<span data-ttu-id="e3c42-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c42-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3c42-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3c42-114">Permission type</span></span> | <span data-ttu-id="e3c42-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3c42-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="e3c42-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3c42-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3c42-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3c42-117">Not Supported</span></span>                       |
| <span data-ttu-id="e3c42-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3c42-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3c42-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e3c42-119">Not Supported</span></span>                       |
| <span data-ttu-id="e3c42-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3c42-120">Application</span></span>     | <span data-ttu-id="e3c42-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e3c42-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="e3c42-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3c42-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="e3c42-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3c42-123">Request headers</span></span>
| <span data-ttu-id="e3c42-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e3c42-124">Name</span></span>          | <span data-ttu-id="e3c42-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c42-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e3c42-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3c42-126">Authorization</span></span> | <span data-ttu-id="e3c42-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3c42-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e3c42-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3c42-129">Content-type</span></span>  | <span data-ttu-id="e3c42-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3c42-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c42-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3c42-132">Request body</span></span>
<span data-ttu-id="e3c42-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e3c42-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3c42-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="e3c42-134">Parameter</span></span>      | <span data-ttu-id="e3c42-135">Тип</span><span class="sxs-lookup"><span data-stu-id="e3c42-135">Type</span></span>    |<span data-ttu-id="e3c42-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e3c42-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c42-137">reason</span><span class="sxs-lookup"><span data-stu-id="e3c42-137">reason</span></span>|<span data-ttu-id="e3c42-138">String</span><span class="sxs-lookup"><span data-stu-id="e3c42-138">String</span></span>|<span data-ttu-id="e3c42-139">Причина отказа.</span><span class="sxs-lookup"><span data-stu-id="e3c42-139">The rejection reason.</span></span> <span data-ttu-id="e3c42-140">Возможные значения: `None` и `Busy``Forbidden`</span><span class="sxs-lookup"><span data-stu-id="e3c42-140">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="e3c42-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="e3c42-141">callbackUri</span></span>|<span data-ttu-id="e3c42-142">String</span><span class="sxs-lookup"><span data-stu-id="e3c42-142">String</span></span>|<span data-ttu-id="e3c42-143">Это позволяет ботам предоставлять определенный URI вызова для текущего вызова для получения более поздних уведомлений.</span><span class="sxs-lookup"><span data-stu-id="e3c42-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="e3c42-144">Если это свойство не установлено, вместо него будет использоваться глобальный URI вызова бота.</span><span class="sxs-lookup"><span data-stu-id="e3c42-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="e3c42-145">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="e3c42-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="e3c42-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3c42-146">Response</span></span>
<span data-ttu-id="e3c42-p108">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3c42-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3c42-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3c42-149">Examples</span></span>
<span data-ttu-id="e3c42-150">В следующих примерах покажите, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="e3c42-150">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="e3c42-151">Пример 1. Отклонение входящих вызовов по причине "занят"</span><span class="sxs-lookup"><span data-stu-id="e3c42-151">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="e3c42-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3c42-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3c42-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c42-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="c"></a>[<span data-ttu-id="e3c42-154">C#</span><span class="sxs-lookup"><span data-stu-id="e3c42-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="e3c42-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3c42-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="e3c42-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3c42-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="java"></a>[<span data-ttu-id="e3c42-157">Java</span><span class="sxs-lookup"><span data-stu-id="e3c42-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="e3c42-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3c42-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="e3c42-159">Пример 2. Отклонение входящих вызовов по причине "Нет"</span><span class="sxs-lookup"><span data-stu-id="e3c42-159">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="e3c42-160">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="e3c42-160">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "name": "call-reject-none",
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
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="e3c42-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3c42-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e3c42-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c42-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="c"></a>[<span data-ttu-id="e3c42-163">C#</span><span class="sxs-lookup"><span data-stu-id="e3c42-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3c42-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3c42-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3c42-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3c42-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3c42-166">Java</span><span class="sxs-lookup"><span data-stu-id="e3c42-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e3c42-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3c42-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="e3c42-168">Уведомление — удалено</span><span class="sxs-lookup"><span data-stu-id="e3c42-168">Notification - deleted</span></span>

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

