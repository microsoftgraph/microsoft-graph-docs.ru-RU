---
title: Получение собраний по сети
description: Получение свойств и связей объекта **онлинемитинг** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ff164b7b525c83436dc5c0db6e583704f79414e3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597017"
---
# <a name="get-online-meeting"></a><span data-ttu-id="a2e30-103">Получение собраний по сети</span><span class="sxs-lookup"><span data-stu-id="a2e30-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e30-104">Получение свойств и связей объекта **онлинемитинг** .</span><span class="sxs-lookup"><span data-stu-id="a2e30-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="a2e30-105">**Примечание:** `GET` Метод ограничен [идентификатором конференции VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Эти идентификаторы создаются для пользователей, лицензированных для облачных видеоконференций, и этот метод используется для получения сведений о присоединении к собранию.</span><span class="sxs-lookup"><span data-stu-id="a2e30-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="a2e30-106">Для обычных потоков, Bot может использовать `joinURL` для присоединения к собранию, а поиск не требуется.</span><span class="sxs-lookup"><span data-stu-id="a2e30-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2e30-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2e30-107">Permissions</span></span>

<span data-ttu-id="a2e30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2e30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2e30-110">Permission type</span></span>                        | <span data-ttu-id="a2e30-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2e30-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="a2e30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2e30-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2e30-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2e30-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="a2e30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2e30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2e30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2e30-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="a2e30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2e30-116">Application</span></span>                            | <span data-ttu-id="a2e30-117">Онлинемитингс. Read. ALL, Онлинемитингс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a2e30-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2e30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2e30-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2e30-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2e30-119">Optional query parameters</span></span>
<span data-ttu-id="a2e30-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a2e30-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2e30-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2e30-121">Request headers</span></span>
| <span data-ttu-id="a2e30-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a2e30-122">Name</span></span>          | <span data-ttu-id="a2e30-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a2e30-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a2e30-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2e30-124">Authorization</span></span> | <span data-ttu-id="a2e30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2e30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2e30-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2e30-127">Request body</span></span>
<span data-ttu-id="a2e30-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2e30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2e30-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2e30-129">Response</span></span>
<span data-ttu-id="a2e30-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онлинемитинг](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2e30-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e30-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a2e30-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a2e30-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2e30-132">Request</span></span>
<span data-ttu-id="a2e30-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2e30-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="a2e30-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2e30-134">Response</span></span>

> <span data-ttu-id="a2e30-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2e30-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
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
  "meetingType": "scheduled",
  "participants": {
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "upn": "upn-value"
      }
    ],
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2e30-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="a2e30-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2e30-138">Языках</span><span class="sxs-lookup"><span data-stu-id="a2e30-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2e30-139">Язык</span><span class="sxs-lookup"><span data-stu-id="a2e30-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
