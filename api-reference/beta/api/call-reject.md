---
title: 'вызов: отклонено'
description: Разрешить интерфейсу Bot отклонить входящий звонок.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e2d14cff71b161b780726c2937b1c008323a9cc5
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302230"
---
# <a name="call-reject"></a><span data-ttu-id="1a798-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="1a798-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a798-104">Разрешить интерфейсу Bot отклонить входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="1a798-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="1a798-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="1a798-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="1a798-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры **чатинфо** и **митингинфо** .</span><span class="sxs-lookup"><span data-stu-id="1a798-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="1a798-107">Ожидается, что Bot отвечает или отклоняет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="1a798-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="1a798-108">Этот API не завершает существующие вызовы, на которые уже получены ответы.</span><span class="sxs-lookup"><span data-stu-id="1a798-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="1a798-109">Чтобы завершить вызов, используйте [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="1a798-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

> <span data-ttu-id="1a798-110">**Примечание:** С помощью VoIP можно получить доступ только через VoIP.</span><span class="sxs-lookup"><span data-stu-id="1a798-110">**Note:** The bot can only be reached through VoIP.</span></span> <span data-ttu-id="1a798-111">Звонки с помощью PSTN в Bot пока не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1a798-111">PSTN calling to bot is not yet supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a798-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a798-112">Permissions</span></span>
<span data-ttu-id="1a798-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a798-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a798-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a798-115">Permission type</span></span> | <span data-ttu-id="1a798-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a798-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="1a798-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a798-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a798-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1a798-118">Not Supported</span></span>                       |
| <span data-ttu-id="1a798-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a798-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a798-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1a798-120">Not Supported</span></span>                       |
| <span data-ttu-id="1a798-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a798-121">Application</span></span>     | <span data-ttu-id="1a798-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1a798-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="1a798-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a798-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="1a798-124">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1a798-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1a798-125">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1a798-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a798-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a798-126">Request headers</span></span>
| <span data-ttu-id="1a798-127">Имя</span><span class="sxs-lookup"><span data-stu-id="1a798-127">Name</span></span>          | <span data-ttu-id="1a798-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1a798-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1a798-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a798-129">Authorization</span></span> | <span data-ttu-id="1a798-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a798-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a798-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a798-132">Content-type</span></span>  | <span data-ttu-id="1a798-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a798-p107">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a798-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a798-135">Request body</span></span>
<span data-ttu-id="1a798-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1a798-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a798-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a798-137">Parameter</span></span>      | <span data-ttu-id="1a798-138">Тип</span><span class="sxs-lookup"><span data-stu-id="1a798-138">Type</span></span>    |<span data-ttu-id="1a798-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1a798-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a798-140">reason</span><span class="sxs-lookup"><span data-stu-id="1a798-140">reason</span></span>|<span data-ttu-id="1a798-141">String</span><span class="sxs-lookup"><span data-stu-id="1a798-141">String</span></span>|<span data-ttu-id="1a798-142">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="1a798-142">The rejection reason.</span></span> <span data-ttu-id="1a798-143">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="1a798-143">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="1a798-144">callbackUri</span><span class="sxs-lookup"><span data-stu-id="1a798-144">callbackUri</span></span>|<span data-ttu-id="1a798-145">String</span><span class="sxs-lookup"><span data-stu-id="1a798-145">String</span></span>|<span data-ttu-id="1a798-146">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="1a798-146">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="1a798-147">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="1a798-147">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="1a798-148">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="1a798-148">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="1a798-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a798-149">Response</span></span>
<span data-ttu-id="1a798-p110">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a798-p110">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a798-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a798-152">Examples</span></span>
<span data-ttu-id="1a798-153">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1a798-153">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="1a798-154">Пример 1: отклонение входящего вызова с причиной "занято"</span><span class="sxs-lookup"><span data-stu-id="1a798-154">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="1a798-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a798-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a798-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a798-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a798-157">C#</span><span class="sxs-lookup"><span data-stu-id="1a798-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a798-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a798-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a798-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a798-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="1a798-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a798-160">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="1a798-161">Пример 2: отклонение входящего вызова с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="1a798-161">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="1a798-162">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="1a798-162">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="1a798-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a798-163">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1a798-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a798-164">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a798-165">C#</span><span class="sxs-lookup"><span data-stu-id="1a798-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a798-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a798-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a798-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a798-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1a798-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a798-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="1a798-169">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="1a798-169">Notification - deleted</span></span>

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
