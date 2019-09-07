---
title: Создание собрания по сети
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6f75891a4ca773f9bcb22bc3a659d9a3a411e3b
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791122"
---
# <a name="create-online-meeting"></a><span data-ttu-id="de2e2-103">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="de2e2-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de2e2-104">Создание собрания по сети от имени пользователя, указанного в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="de2e2-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="de2e2-105">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="de2e2-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="de2e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de2e2-106">Permissions</span></span>
<span data-ttu-id="de2e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de2e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de2e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de2e2-109">Permission type</span></span>                        | <span data-ttu-id="de2e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de2e2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de2e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de2e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de2e2-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de2e2-112">Not Supported</span></span>                               |
| <span data-ttu-id="de2e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de2e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de2e2-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de2e2-114">Not Supported</span></span>                               |
| <span data-ttu-id="de2e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de2e2-115">Application</span></span>                            | <span data-ttu-id="de2e2-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2e2-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="de2e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de2e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="de2e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de2e2-118">Request headers</span></span>
| <span data-ttu-id="de2e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de2e2-119">Name</span></span>          | <span data-ttu-id="de2e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de2e2-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="de2e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de2e2-121">Authorization</span></span> | <span data-ttu-id="de2e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de2e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de2e2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de2e2-124">Request body</span></span>
<span data-ttu-id="de2e2-125">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de2e2-125">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de2e2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="de2e2-126">Response</span></span>
<span data-ttu-id="de2e2-127">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de2e2-127">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de2e2-128">Пример</span><span class="sxs-lookup"><span data-stu-id="de2e2-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="de2e2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="de2e2-129">Request</span></span>
<span data-ttu-id="de2e2-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de2e2-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de2e2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="de2e2-131">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="de2e2-132">C#</span><span class="sxs-lookup"><span data-stu-id="de2e2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de2e2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de2e2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de2e2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de2e2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="de2e2-135">В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de2e2-135">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="de2e2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="de2e2-136">Response</span></span>

><span data-ttu-id="de2e2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de2e2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
