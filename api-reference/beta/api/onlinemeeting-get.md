---
title: Получение собраний по сети
description: Получение свойств и связей объекта собрания по **сети** .
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a96dcefdd98aba1b18c70dfbd0db7609beca74f5
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969160"
---
# <a name="get-online-meeting"></a><span data-ttu-id="48752-103">Получение собраний по сети</span><span class="sxs-lookup"><span data-stu-id="48752-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48752-104">Получение свойств и связей объекта [онлинемитинг](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="48752-104">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="48752-105">**Примечание:** В `GET` настоящее время метод поддерживается только для [идентификатора конференции VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Эти идентификаторы создаются для пользователей, лицензированных для облачных видеоконференций, и этот метод используется для получения сведений о присоединении к собранию.</span><span class="sxs-lookup"><span data-stu-id="48752-105">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="48752-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48752-106">Permissions</span></span>

<span data-ttu-id="48752-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48752-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48752-109">Permission type</span></span>                        | <span data-ttu-id="48752-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48752-110">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="48752-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48752-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48752-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48752-112">Not Supported.</span></span>                                        |
| <span data-ttu-id="48752-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48752-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48752-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48752-114">Not Supported.</span></span>                                        |
| <span data-ttu-id="48752-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48752-115">Application</span></span>                            | <span data-ttu-id="48752-116">Онлинемитингс. Read. ALL, Онлинемитингс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48752-116">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48752-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48752-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```
> <span data-ttu-id="48752-118">**Примечание:** `/app` Путь является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="48752-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="48752-119">Перемотка вперед, используйте `/communications` путь.</span><span class="sxs-lookup"><span data-stu-id="48752-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="48752-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48752-120">Optional query parameters</span></span>
<span data-ttu-id="48752-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="48752-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48752-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48752-122">Request headers</span></span>
| <span data-ttu-id="48752-123">Имя</span><span class="sxs-lookup"><span data-stu-id="48752-123">Name</span></span>          | <span data-ttu-id="48752-124">Описание</span><span class="sxs-lookup"><span data-stu-id="48752-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="48752-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48752-125">Authorization</span></span> | <span data-ttu-id="48752-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48752-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48752-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48752-128">Request body</span></span>
<span data-ttu-id="48752-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48752-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48752-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="48752-130">Response</span></span>
<span data-ttu-id="48752-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онлинемитинг](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48752-131">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48752-132">Пример</span><span class="sxs-lookup"><span data-stu-id="48752-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48752-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48752-133">Request</span></span>
<span data-ttu-id="48752-134">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48752-134">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="48752-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="48752-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48752-136">C#</span><span class="sxs-lookup"><span data-stu-id="48752-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48752-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48752-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48752-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48752-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="48752-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="48752-139">Response</span></span>

> <span data-ttu-id="48752-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48752-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "canceledDateTime": "0001-01-01T08:00:00Z",
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "isBroadcast": false,
  "participants": {
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
            "displayName": "John"
          }
        },
        "upn": "upn-value"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
          "displayName": "Bob"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789"
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
  ]
}
-->
