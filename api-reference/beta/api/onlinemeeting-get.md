---
title: Get собрания по сети
description: Извлечение свойств и связи объекта **onlineMeeting** .
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 75f4b4372e8e2bf12deee4d77f8f271696c715d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880635"
---
# <a name="get-online-meeting"></a><span data-ttu-id="97fd9-103">Get собрания по сети</span><span class="sxs-lookup"><span data-stu-id="97fd9-103">Get Online Meeting</span></span>

> <span data-ttu-id="97fd9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97fd9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97fd9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97fd9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97fd9-106">Извлечение свойств и связи объекта **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="97fd9-106">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="97fd9-107">**Примечание:** `GET` Метод не может превышать [VTC идентификатор конференции](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Эти коды создаются для облачных видео взаимодействия пользователей с корпоративным лицензированием и этот метод используется для получения сведений о присоединиться к собранию.</span><span class="sxs-lookup"><span data-stu-id="97fd9-107">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="97fd9-108">Для регулярного потоков можно использовать робот `joinURL` для присоединения к собранию и без просмотра не требуется.</span><span class="sxs-lookup"><span data-stu-id="97fd9-108">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="97fd9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97fd9-109">Permissions</span></span>

<span data-ttu-id="97fd9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97fd9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97fd9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97fd9-112">Permission type</span></span>                        | <span data-ttu-id="97fd9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97fd9-113">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="97fd9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97fd9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="97fd9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97fd9-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="97fd9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97fd9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97fd9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97fd9-117">Not Supported.</span></span>                                        |
| <span data-ttu-id="97fd9-118">Application</span><span class="sxs-lookup"><span data-stu-id="97fd9-118">Application</span></span>                            | <span data-ttu-id="97fd9-119">OnlineMeetings.Read.All OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97fd9-119">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97fd9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97fd9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97fd9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97fd9-121">Optional query parameters</span></span>
<span data-ttu-id="97fd9-122">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="97fd9-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97fd9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97fd9-123">Request headers</span></span>
| <span data-ttu-id="97fd9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="97fd9-124">Name</span></span>          | <span data-ttu-id="97fd9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="97fd9-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="97fd9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97fd9-126">Authorization</span></span> | <span data-ttu-id="97fd9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97fd9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97fd9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97fd9-129">Request body</span></span>
<span data-ttu-id="97fd9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97fd9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97fd9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="97fd9-131">Response</span></span>
<span data-ttu-id="97fd9-132">Успешно завершена, этот метод возвращает `200 OK` объект [onlineMeeting](../resources/onlinemeeting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="97fd9-132">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97fd9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="97fd9-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97fd9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="97fd9-134">Request</span></span>
<span data-ttu-id="97fd9-135">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97fd9-135">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="97fd9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="97fd9-136">Response</span></span>

> <span data-ttu-id="97fd9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97fd9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
