---
title: Создание собрания по сети
description: Создает собрания от имени пользователя, указанного в тексте запроса.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ac4fb9b378f644e5cf5ba5e9d6412a6ca1fd1b45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946933"
---
# <a name="create-online-meeting"></a><span data-ttu-id="47d29-103">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="47d29-103">Create online meeting</span></span>

> <span data-ttu-id="47d29-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47d29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47d29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d29-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47d29-106">Создает собрания от имени пользователя, указанного в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="47d29-106">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="47d29-107">**Примечание**: собрания не отображается на календарь пользователя.</span><span class="sxs-lookup"><span data-stu-id="47d29-107">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="47d29-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47d29-108">Permissions</span></span>
<span data-ttu-id="47d29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47d29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d29-111">Permission type</span></span>                        | <span data-ttu-id="47d29-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d29-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47d29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d29-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="47d29-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="47d29-114">Not Supported</span></span>                               |
| <span data-ttu-id="47d29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d29-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47d29-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="47d29-116">Not Supported</span></span>                               |
| <span data-ttu-id="47d29-117">Application</span><span class="sxs-lookup"><span data-stu-id="47d29-117">Application</span></span>                            | <span data-ttu-id="47d29-118">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d29-118">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="47d29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d29-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="47d29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47d29-120">Request headers</span></span>
| <span data-ttu-id="47d29-121">Имя</span><span class="sxs-lookup"><span data-stu-id="47d29-121">Name</span></span>          | <span data-ttu-id="47d29-122">Описание</span><span class="sxs-lookup"><span data-stu-id="47d29-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="47d29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47d29-123">Authorization</span></span> | <span data-ttu-id="47d29-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d29-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47d29-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47d29-126">Request body</span></span>
<span data-ttu-id="47d29-127">В тексте запроса укажите представление JSON объекта [onlineMeeting](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="47d29-127">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="47d29-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="47d29-128">Response</span></span>
<span data-ttu-id="47d29-129">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [onlineMeeting](../resources/onlinemeeting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47d29-129">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d29-130">Пример</span><span class="sxs-lookup"><span data-stu-id="47d29-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="47d29-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d29-131">Request</span></span>
<span data-ttu-id="47d29-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d29-132">The following example shows the request.</span></span>

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

<span data-ttu-id="47d29-133">В тексте запроса укажите представление объекта [onlineMeeting](../resources/onlinemeeting.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="47d29-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="47d29-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d29-134">Response</span></span>

><span data-ttu-id="47d29-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47d29-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
