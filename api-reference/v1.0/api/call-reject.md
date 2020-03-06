---
title: 'вызов: отклонено'
description: Разрешить интерфейсу Bot отклонить входящий звонок.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: baa44ba0eec9ef8a4bc9e4111a7c313a26dfa1de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518674"
---
# <a name="call-reject"></a><span data-ttu-id="8b262-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="8b262-103">call: reject</span></span>

<span data-ttu-id="8b262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b262-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b262-105">Разрешить интерфейсу Bot отклонить входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="8b262-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="8b262-106">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="8b262-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="8b262-107">При получении приглашения на вызов группы в уведомлении будут содержаться параметры **чатинфо** и **митингинфо** .</span><span class="sxs-lookup"><span data-stu-id="8b262-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="8b262-108">Ожидается, что Bot отвечает или отклоняет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="8b262-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="8b262-109">Этот API не завершает существующие вызовы, на которые уже получены ответы.</span><span class="sxs-lookup"><span data-stu-id="8b262-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="8b262-110">Чтобы завершить вызов, используйте [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="8b262-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b262-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b262-111">Permissions</span></span>
<span data-ttu-id="8b262-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b262-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b262-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b262-114">Permission type</span></span> | <span data-ttu-id="8b262-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b262-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="8b262-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b262-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b262-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b262-117">Not Supported</span></span>                       |
| <span data-ttu-id="8b262-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b262-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b262-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8b262-119">Not Supported</span></span>                       |
| <span data-ttu-id="8b262-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b262-120">Application</span></span>     | <span data-ttu-id="8b262-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8b262-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="8b262-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b262-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="8b262-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b262-123">Request headers</span></span>
| <span data-ttu-id="8b262-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8b262-124">Name</span></span>          | <span data-ttu-id="8b262-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8b262-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8b262-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b262-126">Authorization</span></span> | <span data-ttu-id="8b262-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b262-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b262-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b262-129">Content-type</span></span>  | <span data-ttu-id="8b262-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b262-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b262-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b262-132">Request body</span></span>
<span data-ttu-id="8b262-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8b262-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b262-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="8b262-134">Parameter</span></span>      | <span data-ttu-id="8b262-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8b262-135">Type</span></span>    |<span data-ttu-id="8b262-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8b262-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b262-137">reason</span><span class="sxs-lookup"><span data-stu-id="8b262-137">reason</span></span>|<span data-ttu-id="8b262-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8b262-138">String</span></span>|<span data-ttu-id="8b262-139">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="8b262-139">The rejection reason.</span></span> <span data-ttu-id="8b262-140">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="8b262-140">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="8b262-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="8b262-141">callbackUri</span></span>|<span data-ttu-id="8b262-142">String</span><span class="sxs-lookup"><span data-stu-id="8b262-142">String</span></span>|<span data-ttu-id="8b262-143">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="8b262-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="8b262-144">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="8b262-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="8b262-145">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="8b262-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="8b262-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b262-146">Response</span></span>
<span data-ttu-id="8b262-p108">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b262-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b262-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b262-149">Examples</span></span>
<span data-ttu-id="8b262-150">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8b262-150">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="8b262-151">Пример 1: отклонение входящего вызова с причиной "занято"</span><span class="sxs-lookup"><span data-stu-id="8b262-151">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="8b262-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b262-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b262-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b262-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b262-154">C#</span><span class="sxs-lookup"><span data-stu-id="8b262-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="8b262-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b262-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="8b262-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b262-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="java"></a>[<span data-ttu-id="8b262-157">Java</span><span class="sxs-lookup"><span data-stu-id="8b262-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="8b262-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b262-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="8b262-159">Пример 2: отклонение входящего вызова с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="8b262-159">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="8b262-160">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="8b262-160">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="8b262-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b262-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b262-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b262-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b262-163">C#</span><span class="sxs-lookup"><span data-stu-id="8b262-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b262-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b262-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b262-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b262-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b262-166">Java</span><span class="sxs-lookup"><span data-stu-id="8b262-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8b262-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b262-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="8b262-168">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="8b262-168">Notification - deleted</span></span>

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
