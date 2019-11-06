---
title: Создание собрания по сети
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: VinodRavichandran
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a63540ee5cb43bf7adf785783780cc97c7cbe658
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968988"
---
# <a name="create-online-meeting"></a><span data-ttu-id="053ab-103">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="053ab-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="053ab-104">Создание собрания по сети от имени пользователя с помощью ИД объекта (oid) в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="053ab-104">Create an online meeting on behalf of a user by using the Object Id (oid) in the user token.</span></span>

> <span data-ttu-id="053ab-105">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="053ab-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="053ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="053ab-106">Permissions</span></span>
<span data-ttu-id="053ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="053ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="053ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="053ab-109">Permission type</span></span>                        | <span data-ttu-id="053ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="053ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="053ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="053ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="053ab-112">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="053ab-112">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="053ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="053ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="053ab-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="053ab-114">Not Supported</span></span>                               |
| <span data-ttu-id="053ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="053ab-115">Application</span></span>                            | <span data-ttu-id="053ab-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053ab-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="053ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="053ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="053ab-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="053ab-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="053ab-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="053ab-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="053ab-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="053ab-120">Request headers</span></span>
| <span data-ttu-id="053ab-121">Имя</span><span class="sxs-lookup"><span data-stu-id="053ab-121">Name</span></span>          | <span data-ttu-id="053ab-122">Описание</span><span class="sxs-lookup"><span data-stu-id="053ab-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="053ab-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="053ab-123">Authorization</span></span> | <span data-ttu-id="053ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="053ab-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="053ab-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="053ab-126">Content-type</span></span>  | <span data-ttu-id="053ab-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="053ab-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="053ab-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="053ab-129">Request body</span></span>
<span data-ttu-id="053ab-130">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="053ab-130">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="053ab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="053ab-131">Response</span></span>
<span data-ttu-id="053ab-132">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="053ab-132">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="053ab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="053ab-133">Example</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="053ab-134">Пример 1. Создание собрания по сети с помощью маркера приложения</span><span class="sxs-lookup"><span data-stu-id="053ab-134">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="053ab-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="053ab-135">Request</span></span>

><span data-ttu-id="053ab-136">**Примечание.** Создание собрания по сети с помощью маркера приложения является устаревшим способом.</span><span class="sxs-lookup"><span data-stu-id="053ab-136">**Note:** Online meeting creation using the application token is deprecated.</span></span> <span data-ttu-id="053ab-137">В дальнейшем используйте путь /me с маркером пользователя, чтобы создавать собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="053ab-137">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="053ab-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="053ab-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-app-token"
}-->
```http
POST https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json

{
  "isBroadcast": "false",
  "startDateTime":"2019-09-09T14:33:30.8546353-07:00",
  "endDateTime":"2019-09-09T15:03:30.8566356-07:00",
  "subject":"Application Token Meeting",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="053ab-139">C#</span><span class="sxs-lookup"><span data-stu-id="053ab-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="053ab-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="053ab-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="053ab-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="053ab-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="053ab-142">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="053ab-142">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="053ab-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="053ab-143">Response</span></span>

><span data-ttu-id="053ab-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="053ab-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "Application Token Meeting"
}
```

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="053ab-146">Пример 2. Создание собрания по сети с помощью маркера пользователя</span><span class="sxs-lookup"><span data-stu-id="053ab-146">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="053ab-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="053ab-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```

#### <a name="response"></a><span data-ttu-id="053ab-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="053ab-148">Response</span></span>
><span data-ttu-id="053ab-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="053ab-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2019-09-14T18:37:29.1973954Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting"
}
```

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="053ab-150">Пример 3. Создание собрания по сети в канале Microsoft Teams с помощью маркера пользователя</span><span class="sxs-lookup"><span data-stu-id="053ab-150">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="053ab-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="053ab-151">Request</span></span>
><span data-ttu-id="053ab-152">**Примечание.** Идентификатор объекта переданного маркера пользователя должен быть элементом канала, представленного с помощью threadid в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="053ab-152">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  }
}
```
#### <a name="response"></a><span data-ttu-id="053ab-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="053ab-153">Response</span></span>

><span data-ttu-id="053ab-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="053ab-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User meeting in Microsoft Teams channel."
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
