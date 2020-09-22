---
title: 'вызов: отклонено'
description: Разрешить интерфейсу Bot отклонить входящий звонок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0c3e711273ab9ca903588a49e310338ca0f9a90d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983391"
---
# <a name="call-reject"></a><span data-ttu-id="d11e9-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="d11e9-103">call: reject</span></span>

<span data-ttu-id="d11e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d11e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11e9-105">Разрешить интерфейсу Bot отклонить входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="d11e9-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="d11e9-106">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="d11e9-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="d11e9-107">При получении приглашения на вызов группы в уведомлении будут содержаться параметры **чатинфо** и **митингинфо** .</span><span class="sxs-lookup"><span data-stu-id="d11e9-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="d11e9-108">Ожидается, что Bot отвечает или отклоняет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="d11e9-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="d11e9-109">Этот API не завершает существующие вызовы, на которые уже получены ответы.</span><span class="sxs-lookup"><span data-stu-id="d11e9-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="d11e9-110">Чтобы завершить вызов, используйте [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="d11e9-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d11e9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d11e9-111">Permissions</span></span>
<span data-ttu-id="d11e9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d11e9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11e9-114">Permission type</span></span> | <span data-ttu-id="d11e9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11e9-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d11e9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11e9-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d11e9-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d11e9-117">Not Supported</span></span>                       |
| <span data-ttu-id="d11e9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11e9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d11e9-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d11e9-119">Not Supported</span></span>                       |
| <span data-ttu-id="d11e9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d11e9-120">Application</span></span>     | <span data-ttu-id="d11e9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d11e9-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="d11e9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11e9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="d11e9-123">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d11e9-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d11e9-124">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d11e9-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d11e9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d11e9-125">Request headers</span></span>
| <span data-ttu-id="d11e9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d11e9-126">Name</span></span>          | <span data-ttu-id="d11e9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d11e9-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d11e9-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d11e9-128">Authorization</span></span> | <span data-ttu-id="d11e9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d11e9-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d11e9-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d11e9-131">Content-type</span></span>  | <span data-ttu-id="d11e9-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d11e9-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d11e9-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11e9-134">Request body</span></span>
<span data-ttu-id="d11e9-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d11e9-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d11e9-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="d11e9-136">Parameter</span></span>      | <span data-ttu-id="d11e9-137">Тип</span><span class="sxs-lookup"><span data-stu-id="d11e9-137">Type</span></span>    |<span data-ttu-id="d11e9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d11e9-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d11e9-139">reason</span><span class="sxs-lookup"><span data-stu-id="d11e9-139">reason</span></span>|<span data-ttu-id="d11e9-140">String</span><span class="sxs-lookup"><span data-stu-id="d11e9-140">String</span></span>|<span data-ttu-id="d11e9-141">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="d11e9-141">The rejection reason.</span></span> <span data-ttu-id="d11e9-142">Возможные значения: `None` `Busy` и `Forbidden`</span><span class="sxs-lookup"><span data-stu-id="d11e9-142">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="d11e9-143">callbackUri</span><span class="sxs-lookup"><span data-stu-id="d11e9-143">callbackUri</span></span>|<span data-ttu-id="d11e9-144">String</span><span class="sxs-lookup"><span data-stu-id="d11e9-144">String</span></span>|<span data-ttu-id="d11e9-145">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="d11e9-145">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="d11e9-146">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="d11e9-146">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="d11e9-147">Это должно быть `https` .</span><span class="sxs-lookup"><span data-stu-id="d11e9-147">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="d11e9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11e9-148">Response</span></span>
<span data-ttu-id="d11e9-p109">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d11e9-p109">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d11e9-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="d11e9-151">Examples</span></span>
<span data-ttu-id="d11e9-152">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d11e9-152">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="d11e9-153">Пример 1: отклонение входящего вызова с причиной "занято"</span><span class="sxs-lookup"><span data-stu-id="d11e9-153">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="d11e9-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11e9-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d11e9-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="d11e9-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d11e9-156">C#</span><span class="sxs-lookup"><span data-stu-id="d11e9-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="d11e9-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d11e9-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="d11e9-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d11e9-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="d11e9-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11e9-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="d11e9-160">Пример 2: отклонение входящего вызова с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="d11e9-160">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d11e9-161">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="d11e9-161">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="d11e9-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11e9-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d11e9-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d11e9-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d11e9-164">C#</span><span class="sxs-lookup"><span data-stu-id="d11e9-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d11e9-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d11e9-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d11e9-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d11e9-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d11e9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11e9-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="d11e9-168">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="d11e9-168">Notification - deleted</span></span>

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


