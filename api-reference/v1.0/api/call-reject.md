---
title: 'вызов: отклонено'
description: Разрешить интерфейсу Bot отклонить входящий звонок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 04ec827cce247e6eef57a025ff81a49ae91353d8
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913704"
---
# <a name="call-reject"></a><span data-ttu-id="588e8-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="588e8-103">call: reject</span></span>

<span data-ttu-id="588e8-104">Разрешить интерфейсу Bot отклонить входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="588e8-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="588e8-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="588e8-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="588e8-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры **чатинфо** и **митингинфо** .</span><span class="sxs-lookup"><span data-stu-id="588e8-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="588e8-107">Ожидается, что Bot отвечает или отклоняет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="588e8-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="588e8-108">Этот API не завершает существующие вызовы, на которые уже получены ответы.</span><span class="sxs-lookup"><span data-stu-id="588e8-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="588e8-109">Чтобы завершить вызов, используйте [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="588e8-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="588e8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="588e8-110">Permissions</span></span>
<span data-ttu-id="588e8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="588e8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588e8-113">Permission type</span></span> | <span data-ttu-id="588e8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="588e8-114">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="588e8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588e8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="588e8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="588e8-116">Not Supported</span></span>                       |
| <span data-ttu-id="588e8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588e8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588e8-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="588e8-118">Not Supported</span></span>                       |
| <span data-ttu-id="588e8-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588e8-119">Application</span></span>     | <span data-ttu-id="588e8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="588e8-120">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="588e8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588e8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="588e8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="588e8-122">Request headers</span></span>
| <span data-ttu-id="588e8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="588e8-123">Name</span></span>          | <span data-ttu-id="588e8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="588e8-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="588e8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588e8-125">Authorization</span></span> | <span data-ttu-id="588e8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588e8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="588e8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="588e8-128">Content-type</span></span>  | <span data-ttu-id="588e8-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588e8-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="588e8-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="588e8-131">Request body</span></span>
<span data-ttu-id="588e8-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="588e8-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="588e8-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="588e8-133">Parameter</span></span>      | <span data-ttu-id="588e8-134">Тип</span><span class="sxs-lookup"><span data-stu-id="588e8-134">Type</span></span>    |<span data-ttu-id="588e8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="588e8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="588e8-136">reason</span><span class="sxs-lookup"><span data-stu-id="588e8-136">reason</span></span>|<span data-ttu-id="588e8-137">String</span><span class="sxs-lookup"><span data-stu-id="588e8-137">String</span></span>|<span data-ttu-id="588e8-138">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="588e8-138">The rejection reason.</span></span> <span data-ttu-id="588e8-139">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="588e8-139">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="588e8-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="588e8-140">callbackUri</span></span>|<span data-ttu-id="588e8-141">String</span><span class="sxs-lookup"><span data-stu-id="588e8-141">String</span></span>|<span data-ttu-id="588e8-142">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="588e8-142">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="588e8-143">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="588e8-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="588e8-144">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="588e8-144">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="588e8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="588e8-145">Response</span></span>
<span data-ttu-id="588e8-p108">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="588e8-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="588e8-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="588e8-148">Examples</span></span>
<span data-ttu-id="588e8-149">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="588e8-149">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="588e8-150">Пример 1: отклонение входящего вызова с причиной "занято"</span><span class="sxs-lookup"><span data-stu-id="588e8-150">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="588e8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="588e8-151">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="588e8-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="588e8-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="588e8-153">C#</span><span class="sxs-lookup"><span data-stu-id="588e8-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="588e8-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="588e8-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="588e8-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="588e8-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javatabjava"></a>[<span data-ttu-id="588e8-156">Java</span><span class="sxs-lookup"><span data-stu-id="588e8-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="588e8-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="588e8-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="588e8-158">Пример 2: отклонение входящего вызова с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="588e8-158">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="588e8-159">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="588e8-159">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="588e8-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="588e8-160">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="588e8-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="588e8-161">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="588e8-162">C#</span><span class="sxs-lookup"><span data-stu-id="588e8-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="588e8-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="588e8-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="588e8-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="588e8-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="588e8-165">Java</span><span class="sxs-lookup"><span data-stu-id="588e8-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="588e8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="588e8-166">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="588e8-167">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="588e8-167">Notification - deleted</span></span>

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
