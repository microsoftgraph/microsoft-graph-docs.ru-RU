---
title: Get собрания по сети
description: Извлечение свойств и связи объекта **onlineMeeting** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ef45d73aef8124d962d05ea84117c93bac16f0a2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510654"
---
# <a name="get-online-meeting"></a><span data-ttu-id="0ccf5-103">Get собрания по сети</span><span class="sxs-lookup"><span data-stu-id="0ccf5-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ccf5-104">Извлечение свойств и связи объекта **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="0ccf5-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="0ccf5-105">**Примечание:** `GET` Метод не может превышать [VTC идентификатор конференции](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Эти коды создаются для облачных видео взаимодействия пользователей с корпоративным лицензированием и этот метод используется для получения сведений о присоединиться к собранию.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="0ccf5-106">Для регулярного потоков можно использовать робот `joinURL` для присоединения к собранию и без просмотра не требуется.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ccf5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccf5-107">Permissions</span></span>

<span data-ttu-id="0ccf5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ccf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ccf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccf5-110">Permission type</span></span>                        | <span data-ttu-id="0ccf5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ccf5-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="0ccf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ccf5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ccf5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="0ccf5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ccf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ccf5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="0ccf5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ccf5-116">Application</span></span>                            | <span data-ttu-id="0ccf5-117">OnlineMeetings.Read.All OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ccf5-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ccf5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ccf5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ccf5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ccf5-119">Optional query parameters</span></span>
<span data-ttu-id="0ccf5-120">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ccf5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ccf5-121">Request headers</span></span>
| <span data-ttu-id="0ccf5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0ccf5-122">Name</span></span>          | <span data-ttu-id="0ccf5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0ccf5-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0ccf5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ccf5-124">Authorization</span></span> | <span data-ttu-id="0ccf5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ccf5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ccf5-127">Request body</span></span>
<span data-ttu-id="0ccf5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ccf5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ccf5-129">Response</span></span>
<span data-ttu-id="0ccf5-130">Успешно завершена, этот метод возвращает `200 OK` объект [onlineMeeting](../resources/onlinemeeting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccf5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ccf5-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ccf5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ccf5-132">Request</span></span>
<span data-ttu-id="0ccf5-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="0ccf5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ccf5-134">Response</span></span>

> <span data-ttu-id="0ccf5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ccf5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
