---
title: Создание собрания по сети
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: bd4d68a5e93e9b1b0afe91129d83e40135e79cbf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258431"
---
# <a name="create-online-meeting"></a><span data-ttu-id="c2480-103">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="c2480-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2480-104">Создание собрания по сети от имени пользователя, указанного в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="c2480-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="c2480-105">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2480-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2480-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2480-106">Permissions</span></span>
<span data-ttu-id="c2480-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2480-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2480-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2480-109">Permission type</span></span>                        | <span data-ttu-id="c2480-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2480-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2480-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2480-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2480-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2480-112">Not Supported</span></span>                               |
| <span data-ttu-id="c2480-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2480-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2480-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c2480-114">Not Supported</span></span>                               |
| <span data-ttu-id="c2480-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2480-115">Application</span></span>                            | <span data-ttu-id="c2480-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2480-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="c2480-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2480-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="c2480-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2480-118">Request headers</span></span>
| <span data-ttu-id="c2480-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c2480-119">Name</span></span>          | <span data-ttu-id="c2480-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c2480-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c2480-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2480-121">Authorization</span></span> | <span data-ttu-id="c2480-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2480-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2480-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2480-124">Request body</span></span>
<span data-ttu-id="c2480-125">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2480-125">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c2480-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2480-126">Response</span></span>
<span data-ttu-id="c2480-127">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2480-127">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2480-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c2480-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2480-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2480-129">Request</span></span>
<span data-ttu-id="c2480-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2480-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

<span data-ttu-id="c2480-131">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2480-131">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c2480-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2480-132">Response</span></span>

><span data-ttu-id="c2480-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2480-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1574

{
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "meetNow",
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
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2480-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c2480-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2480-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2480-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2480-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2480-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2480-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2480-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-onlinemeeting-from-application-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
