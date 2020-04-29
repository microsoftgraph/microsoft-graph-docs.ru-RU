---
title: Получение Онлинемитинг
description: Получение свойств и связей объекта собрания по **сети** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 948f05e97471bd9be6442dade4fe55f6b1e90e7b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917115"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="1bf23-103">Получение Онлинемитинг</span><span class="sxs-lookup"><span data-stu-id="1bf23-103">Get onlineMeeting</span></span>

<span data-ttu-id="1bf23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bf23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bf23-105">Получение свойств и связей объекта [онлинемитинг](../resources/onlinemeeting.md) .</span><span class="sxs-lookup"><span data-stu-id="1bf23-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="1bf23-106">**Примечание:** В `GET` настоящее время метод поддерживается только для [идентификатора конференции VTC](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). Эти идентификаторы создаются для пользователей, лицензированных для облачных видеоконференций, и этот метод используется для получения сведений о присоединении к собранию.</span><span class="sxs-lookup"><span data-stu-id="1bf23-106">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bf23-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf23-107">Permissions</span></span>

<span data-ttu-id="1bf23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bf23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1bf23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf23-110">Permission type</span></span>                        | <span data-ttu-id="1bf23-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bf23-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="1bf23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bf23-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1bf23-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf23-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="1bf23-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bf23-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bf23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf23-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="1bf23-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bf23-116">Application</span></span>                            | <span data-ttu-id="1bf23-117">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bf23-117">OnlineMeetings.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bf23-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bf23-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bf23-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1bf23-119">Optional query parameters</span></span>
<span data-ttu-id="1bf23-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1bf23-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bf23-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bf23-121">Request headers</span></span>
| <span data-ttu-id="1bf23-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1bf23-122">Name</span></span>          | <span data-ttu-id="1bf23-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf23-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1bf23-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bf23-124">Authorization</span></span> | <span data-ttu-id="1bf23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bf23-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bf23-127">Request body</span></span>
<span data-ttu-id="1bf23-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bf23-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bf23-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bf23-129">Response</span></span>
<span data-ttu-id="1bf23-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bf23-130">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1bf23-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bf23-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1bf23-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bf23-132">Request</span></span>
<span data-ttu-id="1bf23-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bf23-133">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1bf23-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bf23-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="1bf23-135">C#</span><span class="sxs-lookup"><span data-stu-id="1bf23-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bf23-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bf23-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bf23-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bf23-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bf23-138">Java</span><span class="sxs-lookup"><span data-stu-id="1bf23-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1bf23-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bf23-139">Response</span></span>

> <span data-ttu-id="1bf23-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bf23-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "55525634478",
    "tollFreeNumber": "55566390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
  "@odata.type": "#microsoft.graph.meetingParticipants",
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "displayName": "Tyler Stein"
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
          "displayName": "Jasmine Miller"
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
