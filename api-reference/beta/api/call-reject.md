---
title: 'вызов: отклонено'
description: Разрешить интерфейсу Bot отклонить входящий звонок.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a083459a162117addba494f74e50842435a74516
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005917"
---
# <a name="call-reject"></a><span data-ttu-id="d69b3-103">вызов: отклонено</span><span class="sxs-lookup"><span data-stu-id="d69b3-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d69b3-104">Разрешить интерфейсу Bot отклонить входящий звонок.</span><span class="sxs-lookup"><span data-stu-id="d69b3-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="d69b3-105">Запрос входящего вызова может быть приглашенным из участника группы или однорангового вызова.</span><span class="sxs-lookup"><span data-stu-id="d69b3-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="d69b3-106">При получении приглашения на вызов группы в уведомлении будут содержаться параметры **чатинфо** и **митингинфо** .</span><span class="sxs-lookup"><span data-stu-id="d69b3-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="d69b3-107">Ожидается, что Bot отвечает или отклоняет вызов до истечения времени ожидания вызова. Текущее значение времени ожидания — 15 секунд.</span><span class="sxs-lookup"><span data-stu-id="d69b3-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="d69b3-108">Этот API не завершает существующие вызовы, на которые уже получены ответы.</span><span class="sxs-lookup"><span data-stu-id="d69b3-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="d69b3-109">Чтобы завершить вызов, используйте [Вызов delete](../api/call-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="d69b3-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

> <span data-ttu-id="d69b3-110">**Примечание:** С помощью VoIP можно получить доступ только через VoIP.</span><span class="sxs-lookup"><span data-stu-id="d69b3-110">**Note:** The bot can only be reached through VoIP.</span></span> <span data-ttu-id="d69b3-111">Звонки с помощью PSTN в Bot пока не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d69b3-111">PSTN calling to bot is not yet supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="d69b3-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d69b3-112">Permissions</span></span>
<span data-ttu-id="d69b3-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d69b3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d69b3-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d69b3-115">Permission type</span></span> | <span data-ttu-id="d69b3-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d69b3-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d69b3-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d69b3-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d69b3-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d69b3-118">Not Supported</span></span>                       |
| <span data-ttu-id="d69b3-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d69b3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d69b3-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d69b3-120">Not Supported</span></span>                       |
| <span data-ttu-id="d69b3-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d69b3-121">Application</span></span>     | <span data-ttu-id="d69b3-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d69b3-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="d69b3-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d69b3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="d69b3-124">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="d69b3-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d69b3-125">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="d69b3-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d69b3-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d69b3-126">Request headers</span></span>
| <span data-ttu-id="d69b3-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d69b3-127">Name</span></span>          | <span data-ttu-id="d69b3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d69b3-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d69b3-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d69b3-129">Authorization</span></span> | <span data-ttu-id="d69b3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d69b3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d69b3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d69b3-132">Content-type</span></span>  | <span data-ttu-id="d69b3-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d69b3-p107">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d69b3-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d69b3-135">Request body</span></span>
<span data-ttu-id="d69b3-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d69b3-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d69b3-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="d69b3-137">Parameter</span></span>      | <span data-ttu-id="d69b3-138">Тип</span><span class="sxs-lookup"><span data-stu-id="d69b3-138">Type</span></span>    |<span data-ttu-id="d69b3-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d69b3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d69b3-140">reason</span><span class="sxs-lookup"><span data-stu-id="d69b3-140">reason</span></span>|<span data-ttu-id="d69b3-141">String</span><span class="sxs-lookup"><span data-stu-id="d69b3-141">String</span></span>|<span data-ttu-id="d69b3-142">Причина отклонения.</span><span class="sxs-lookup"><span data-stu-id="d69b3-142">The rejection reason.</span></span> <span data-ttu-id="d69b3-143">Возможные значения: `None` `Busy` и`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="d69b3-143">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="d69b3-144">callbackUri</span><span class="sxs-lookup"><span data-stu-id="d69b3-144">callbackUri</span></span>|<span data-ttu-id="d69b3-145">String</span><span class="sxs-lookup"><span data-stu-id="d69b3-145">String</span></span>|<span data-ttu-id="d69b3-146">Это позволяет Боты предоставить определенный URI обратного вызова для текущего вызова, чтобы получать уведомления позже.</span><span class="sxs-lookup"><span data-stu-id="d69b3-146">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="d69b3-147">Если это свойство не задано, вместо него будет использоваться глобальный URI обратного вызова Bot.</span><span class="sxs-lookup"><span data-stu-id="d69b3-147">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="d69b3-148">Это должно быть `https`.</span><span class="sxs-lookup"><span data-stu-id="d69b3-148">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="d69b3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d69b3-149">Response</span></span>
<span data-ttu-id="d69b3-p110">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d69b3-p110">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d69b3-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="d69b3-152">Examples</span></span>
<span data-ttu-id="d69b3-153">В следующих примерах показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d69b3-153">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="d69b3-154">Пример 1: отклонение входящего вызова с причиной "занято"</span><span class="sxs-lookup"><span data-stu-id="d69b3-154">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="d69b3-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d69b3-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d69b3-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="d69b3-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d69b3-157">C#</span><span class="sxs-lookup"><span data-stu-id="d69b3-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d69b3-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d69b3-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d69b3-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d69b3-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="d69b3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="d69b3-160">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="d69b3-161">Пример 2: отклонение входящего вызова с причиной "нет"</span><span class="sxs-lookup"><span data-stu-id="d69b3-161">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="d69b3-162">Уведомление — входящий</span><span class="sxs-lookup"><span data-stu-id="d69b3-162">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="d69b3-163">Запросить</span><span class="sxs-lookup"><span data-stu-id="d69b3-163">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d69b3-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="d69b3-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="d69b3-165">Уведомление удалено</span><span class="sxs-lookup"><span data-stu-id="d69b3-165">Notification - deleted</span></span>

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
