---
title: Создание объекта onlineMeeting
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f3195f55532713ee4bc359623b8fed241b799f3f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441475"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="1ff6b-103">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1ff6b-103">Create onlineMeeting</span></span>

<span data-ttu-id="1ff6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ff6b-105">Создание собрания по сети от имени пользователя с помощью ИД объекта (OID) в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-105">Create an online meeting on behalf of a user by using the object ID (OID) in the user token.</span></span>

> <span data-ttu-id="1ff6b-106">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-106">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff6b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff6b-107">Permissions</span></span>
<span data-ttu-id="1ff6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ff6b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff6b-110">Permission type</span></span>                        | <span data-ttu-id="1ff6b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ff6b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ff6b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ff6b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ff6b-113">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ff6b-113">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="1ff6b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ff6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff6b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1ff6b-115">Not Supported</span></span>                               |
| <span data-ttu-id="1ff6b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ff6b-116">Application</span></span>                            | <span data-ttu-id="1ff6b-117">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="1ff6b-117">OnlineMeetings.ReadWrite.All\*</span></span>  |

> <span data-ttu-id="1ff6b-118">\* **Примечание.** Поддержка разрешений приложений прекращается, и они будут удалены в апреле 2020 г.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-118">\* **Note:** Application permissions are deprecated and will be removed in April 2020.</span></span>

## <a name="http-request"></a><span data-ttu-id="1ff6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ff6b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="1ff6b-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1ff6b-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff6b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ff6b-122">Request headers</span></span>
| <span data-ttu-id="1ff6b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1ff6b-123">Name</span></span>          | <span data-ttu-id="1ff6b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1ff6b-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1ff6b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ff6b-125">Authorization</span></span> | <span data-ttu-id="1ff6b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ff6b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ff6b-128">Content-type</span></span>  | <span data-ttu-id="1ff6b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ff6b-131">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ff6b-131">Request body</span></span>
<span data-ttu-id="1ff6b-132">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-132">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ff6b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff6b-133">Response</span></span>
<span data-ttu-id="1ff6b-134">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-134">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ff6b-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ff6b-135">Examples</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="1ff6b-136">Пример 1. Создание собрания по сети с помощью маркера приложения</span><span class="sxs-lookup"><span data-stu-id="1ff6b-136">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="1ff6b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff6b-137">Request</span></span>

> [!Note]
> <span data-ttu-id="1ff6b-138">Создание собрания по сети с помощью маркера приложения является устаревшим способом, и его поддержка будет прекращена в апреле 2020 г.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-138">Online meeting creation using an application token is deprecated and support will be removed in April 2020.</span></span> <span data-ttu-id="1ff6b-139">В дальнейшем используйте путь /me с маркером пользователя, чтобы создавать собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-139">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff6b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff6b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-app-token"
}-->
```http
POST https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json

{
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
# <a name="c"></a>[<span data-ttu-id="1ff6b-141">C#</span><span class="sxs-lookup"><span data-stu-id="1ff6b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff6b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff6b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff6b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff6b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="1ff6b-144">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-144">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="1ff6b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff6b-145">Response</span></span>

><span data-ttu-id="1ff6b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
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

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="1ff6b-148">Пример 2. Создание собрания по сети с помощью маркера пользователя</span><span class="sxs-lookup"><span data-stu-id="1ff6b-148">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="1ff6b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff6b-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff6b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff6b-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1ff6b-151">C#</span><span class="sxs-lookup"><span data-stu-id="1ff6b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff6b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff6b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff6b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff6b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1ff6b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff6b-154">Response</span></span>
><span data-ttu-id="1ff6b-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-155">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
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

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="1ff6b-156">Пример 3. Создание собрания по сети в канале Microsoft Teams с помощью маркера пользователя</span><span class="sxs-lookup"><span data-stu-id="1ff6b-156">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="1ff6b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff6b-157">Request</span></span>
><span data-ttu-id="1ff6b-158">**Примечание.** Идентификатор объекта переданного маркера пользователя должен быть элементом канала, представленного с помощью threadid в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-158">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

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
#### <a name="response"></a><span data-ttu-id="1ff6b-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff6b-159">Response</span></span>

><span data-ttu-id="1ff6b-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ff6b-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
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
