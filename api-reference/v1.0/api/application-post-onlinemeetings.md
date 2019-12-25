---
title: Создание объекта onlineMeeting
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: VinodRavichandran
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a4c044dccf07a20cf697912fc0e135ea5951fca1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866350"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="770fa-103">Создание объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="770fa-103">Create onlineMeeting</span></span>

<span data-ttu-id="770fa-104">Создание собрания по сети от имени пользователя с помощью ИД объекта (OID) в маркере пользователя.</span><span class="sxs-lookup"><span data-stu-id="770fa-104">Create an online meeting on behalf of a user by using the Object Id (oid) in the user token.</span></span>

> <span data-ttu-id="770fa-105">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="770fa-105">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="770fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="770fa-106">Permissions</span></span>
<span data-ttu-id="770fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="770fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="770fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="770fa-109">Permission type</span></span>                        | <span data-ttu-id="770fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="770fa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="770fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="770fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="770fa-112">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="770fa-112">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="770fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="770fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="770fa-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="770fa-114">Not Supported</span></span>                               |
| <span data-ttu-id="770fa-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="770fa-115">Application</span></span>                            | <span data-ttu-id="770fa-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="770fa-116">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="770fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="770fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="770fa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="770fa-118">Request headers</span></span>
| <span data-ttu-id="770fa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="770fa-119">Name</span></span>          | <span data-ttu-id="770fa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="770fa-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="770fa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="770fa-121">Authorization</span></span> | <span data-ttu-id="770fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="770fa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="770fa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="770fa-124">Content-type</span></span>  | <span data-ttu-id="770fa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="770fa-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="770fa-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="770fa-127">Request body</span></span>
<span data-ttu-id="770fa-128">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="770fa-128">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="770fa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="770fa-129">Response</span></span>
<span data-ttu-id="770fa-130">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="770fa-130">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="770fa-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="770fa-131">Examples</span></span> 

<span data-ttu-id="770fa-132">В приведенном ниже примере показано, как создать собрание по сети с помощью маркера пользователя.</span><span class="sxs-lookup"><span data-stu-id="770fa-132">The following example creates an online meeting with a user token.</span></span>

### <a name="request"></a><span data-ttu-id="770fa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="770fa-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="770fa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="770fa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="770fa-135">C#</span><span class="sxs-lookup"><span data-stu-id="770fa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="770fa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="770fa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="770fa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="770fa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="770fa-138">Java</span><span class="sxs-lookup"><span data-stu-id="770fa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onlinemeeting-user-token-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="770fa-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="770fa-139">Response</span></span>
><span data-ttu-id="770fa-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="770fa-140">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
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
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting"
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
