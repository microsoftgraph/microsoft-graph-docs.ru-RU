---
title: Get onlineMeeting
description: Извлечение свойств и связей объекта onlineMeeting.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f156adc43759ae6bdbeb10b7857e39157033c68c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866125"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="8d3e0-103">Get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8d3e0-103">Get onlineMeeting</span></span>

<span data-ttu-id="8d3e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d3e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d3e0-105">Извлечение свойств и связей объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="8d3e0-106">Например, вы можете:</span><span class="sxs-lookup"><span data-stu-id="8d3e0-106">For example, you can:</span></span>
- <span data-ttu-id="8d3e0-107">Получите сведения об onlineMeeting с помощью [VideoTeleconferenceId,](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid) [ИД](#example-2-retrieve-an-online-meeting-by-meeting-id)собрания или [JoinWebURL.](#example-3-retrieve-an-online-meeting-by-joinweburl)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-107">Get details of an onlineMeeting using [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid), [meeting ID](#example-2-retrieve-an-online-meeting-by-meeting-id), or [JoinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl).</span></span>
- <span data-ttu-id="8d3e0-108">Используйте `/attendeeReport` путь, чтобы получить отчет участника о трансляции, как показано [в примере 4.](#example-4-retrieve-the-attendee-report-of-a-live-event)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-108">Use the `/attendeeReport` path to get an attendee report of a live event, as shown in [example 4](#example-4-retrieve-the-attendee-report-of-a-live-event).</span></span>
- <span data-ttu-id="8d3e0-109">Используйте эти пути для получения записей трансляции, как показано `/recording` `/alternativeRecording` в [примере 5.](#example-5-retrieve-the-recording-of-a-live-event)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-109">Use the `/recording` and `/alternativeRecording` paths to get the recordings of a live event, as shown in [example 5](#example-5-retrieve-the-recording-of-a-live-event).</span></span>

><span data-ttu-id="8d3e0-110">**Примечания:**</span><span class="sxs-lookup"><span data-stu-id="8d3e0-110">**Notes:**</span></span> 
>- <span data-ttu-id="8d3e0-111">В настоящее время отчеты и записи участников доступны только для трансляций.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-111">Currently, attendee reports and recordings are available only to live events.</span></span>
>- <span data-ttu-id="8d3e0-112">Только организатор событий может получить доступ к отчетам и записям участников.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-112">Only the event organizer can access attendee reports and recordings.</span></span>
>- <span data-ttu-id="8d3e0-113">Отчеты и записи участников доступны только после того, как завершилось трансляция.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-113">Attendee reports and recordings are only available when the live event has concluded.</span></span>
>- <span data-ttu-id="8d3e0-114">Срок действия ссылки для `302 Found` [скачивания в ответе](#example-4-retrieve-the-attendee-report-of-a-live-event) истекает **через 60** секунд.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-114">The download link in the `302 Found` [response](#example-4-retrieve-the-attendee-report-of-a-live-event) expires in **60** seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d3e0-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3e0-115">Permissions</span></span>

<span data-ttu-id="8d3e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d3e0-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3e0-118">Permission type</span></span>                        | <span data-ttu-id="8d3e0-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-119">Permissions (from least to most privileged)</span></span>           |
| :------------------------------------- | :---------------------------------------------------- |
| <span data-ttu-id="8d3e0-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d3e0-121">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d3e0-121">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span></span>         |
| <span data-ttu-id="8d3e0-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3e0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-123">Not Supported.</span></span>                                        |
| <span data-ttu-id="8d3e0-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d3e0-124">Application</span></span>                            | <span data-ttu-id="8d3e0-125">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="8d3e0-125">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="8d3e0-126">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, разрешив приложению, настроенном в политике, получать собрание по сети от имени этого пользователя (ид пользователя, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="8d3e0-126">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to retrieve an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="8d3e0-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-127">HTTP request</span></span>

<span data-ttu-id="8d3e0-128">Чтобы получить указанный onlineMeeting с помощью ИД собрания:</span><span class="sxs-lookup"><span data-stu-id="8d3e0-128">To get the specified onlineMeeting using meeting ID:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}
GET /users/{userId}/onlineMeetings/{meetingId}
```

<span data-ttu-id="8d3e0-129">Чтобы получить указанный onlineMeeting с **помощью videoTeleconferenceId:**</span><span class="sxs-lookup"><span data-stu-id="8d3e0-129">To get the specified onlineMeeting using **videoTeleconferenceId**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```

<span data-ttu-id="8d3e0-130">Чтобы получить указанное onlineMeeting с **помощью joinWebUrl:**</span><span class="sxs-lookup"><span data-stu-id="8d3e0-130">To get the specified onlineMeeting using **joinWebUrl**:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
```

<span data-ttu-id="8d3e0-131">Чтобы получить отчет об участниках трансляции:</span><span class="sxs-lookup"><span data-stu-id="8d3e0-131">To get the attendee report of a live event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}/attendeeReport
```

<span data-ttu-id="8d3e0-132">Чтобы получить записи трансляции:</span><span class="sxs-lookup"><span data-stu-id="8d3e0-132">To get the recordings of a live event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}/recording
GET /users/{userId}/onlineMeetings/{meetingId}/alternativeRecording
```

><span data-ttu-id="8d3e0-133">**Примечания:**</span><span class="sxs-lookup"><span data-stu-id="8d3e0-133">**Notes:**</span></span>
>- <span data-ttu-id="8d3e0-134">Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-134">The `/app` path is deprecated.</span></span> <span data-ttu-id="8d3e0-135">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-135">Going forward, use the `/communications` path.</span></span>
>- <span data-ttu-id="8d3e0-136">`id`в первых двух маршрутах указывается ИД [конференции VTC.](/microsoftteams/cloud-video-interop-for-teams-set-up)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-136">`id` in the first two routes refers to [VTC conference id](/microsoftteams/cloud-video-interop-for-teams-set-up).</span></span>
>- <span data-ttu-id="8d3e0-137">`userId`— это ИД объекта пользователя на портале [управления пользователями Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-137">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="8d3e0-138">Дополнительные сведения [см. в политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-138">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
>- <span data-ttu-id="8d3e0-139">`meetingId`— **это ид** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-139">`meetingId` is the **id** of an [onlineMeeting entity](../resources/onlinemeeting.md).</span></span>
>- <span data-ttu-id="8d3e0-140">`joinWebUrl` должен быть закодирован с помощью URL-адреса, и этот маршрут можно использовать только для получения собраний, созданных с помощью `userId` .</span><span class="sxs-lookup"><span data-stu-id="8d3e0-140">`joinWebUrl` must be URL encoded and this route can only be used to retrieve meetings created by `userId`.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8d3e0-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d3e0-141">Optional query parameters</span></span>
<span data-ttu-id="8d3e0-142">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-142">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d3e0-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d3e0-143">Request headers</span></span>
| <span data-ttu-id="8d3e0-144">Имя</span><span class="sxs-lookup"><span data-stu-id="8d3e0-144">Name</span></span>            | <span data-ttu-id="8d3e0-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3e0-145">Description</span></span>               |
| :-------------- | :------------------------ |
| <span data-ttu-id="8d3e0-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d3e0-146">Authorization</span></span>   | <span data-ttu-id="8d3e0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d3e0-149">Принять-Язык</span><span class="sxs-lookup"><span data-stu-id="8d3e0-149">Accept-Language</span></span> | <span data-ttu-id="8d3e0-150">Язык.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-150">Language.</span></span> <span data-ttu-id="8d3e0-151">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-151">Optional.</span></span>       |

<span data-ttu-id="8d3e0-152">Если запрос содержит `Accept-Language` HTTP-заголовок, то `content` из `joinInformation` будет указан на языке и языкового стандарта, указанного в заголовке `Accept-Language`.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-152">If the request contains an `Accept-Language` HTTP header, the `content` of `joinInformation` will be in the language and locale variant specified in the `Accept-Language` header.</span></span> <span data-ttu-id="8d3e0-153">Контент по умолчанию будет на английском языке.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-153">The default content will be in English.</span></span>

## <a name="request-body"></a><span data-ttu-id="8d3e0-154">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d3e0-154">Request body</span></span>
<span data-ttu-id="8d3e0-155">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3e0-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-156">Response</span></span>
<span data-ttu-id="8d3e0-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-157">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="8d3e0-158">Метод также включает одно из следующих:</span><span class="sxs-lookup"><span data-stu-id="8d3e0-158">The method also includes one of the following:</span></span>

- <span data-ttu-id="8d3e0-159">Если вы получаете собрание по сети на основе ИД собрания, **videoTeleconferenceId** или **joinWebUrl,** этот метод также возвращает объект [onlineMeeting](../resources/onlinemeeting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-159">If you're getting an online meeting based on meeting ID, **videoTeleconferenceId** or **joinWebUrl**, this method also returns an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>
- <span data-ttu-id="8d3e0-160">Если вы получаете отчет об участниках или запись собрания по сети, этот метод также возвращает заглавную запись, которая указывает URI отчету или записи участника `Location` соответственно.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-160">If you're getting the attendee report or recording of a live online meeting, this method also returns a `Location` header that indicates the URI to the attendee report or recording, respectively.</span></span>

## <a name="examples"></a><span data-ttu-id="8d3e0-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d3e0-161">Examples</span></span>

### <a name="example-1-retrieve-an-online-meeting-by-videoteleconferenceid"></a><span data-ttu-id="8d3e0-162">Пример 1. Извлечение собрания по сети с помощью VideoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="8d3e0-162">Example 1: Retrieve an online meeting by VideoTeleconferenceId</span></span>

#### <a name="request"></a><span data-ttu-id="8d3e0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-163">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8d3e0-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d3e0-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="8d3e0-165">C#</span><span class="sxs-lookup"><span data-stu-id="8d3e0-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d3e0-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d3e0-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d3e0-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d3e0-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d3e0-168">Java</span><span class="sxs-lookup"><span data-stu-id="8d3e0-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8d3e0-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-169">Response</span></span>

> <span data-ttu-id="8d3e0-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
            "displayName": "Tyler Stein"
          }
        },
        "upn": "upn-value",
        "role": "attendee"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
          "displayName": "Jasmine Miller"
        }
      },
      "upn": "upn-value",
      "role": "presenter"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789",
  "lobbyBypassSettings": {
    "scope": "everyone",
    "isDialInBypassEnabled": true
  },
  "isEntryExitAnnounced": true,
  "allowedPresenters": "everyone"
}
```
><span data-ttu-id="8d3e0-172">**Примечание.** если указан японский язык, в ответ будут включены перечисленные ниже данные.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-172">**Note:** If 'Accept-Language: ja' is specified to indicate Japanese, for example, the response will include the following.</span></span>

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```

### <a name="example-2-retrieve-an-online-meeting-by-meeting-id"></a><span data-ttu-id="8d3e0-173">Пример 2. Извлечение онлайн-собрания по его ИД</span><span class="sxs-lookup"><span data-stu-id="8d3e0-173">Example 2: Retrieve an online meeting by meeting ID</span></span>
<span data-ttu-id="8d3e0-174">Вы можете получить сведения о собрании с помощью ИД собрания с помощью маркера пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-174">You can retrieve meeting information via meeting ID with either a user or application token.</span></span> <span data-ttu-id="8d3e0-175">При создании объекта [onlineMeeting](../resources/onlinemeeting.md)в объекте ответа предоставляется ИД собрания.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-175">The meeting ID is provided in the response object when creating an [onlineMeeting](../resources/onlinemeeting.md).</span></span> <span data-ttu-id="8d3e0-176">Этот параметр доступен для поддержки случаев использования, когда известен ИД собрания, например, когда приложение сначала создает собрание, а затем извлекает сведения о собрании позже в качестве отдельного действия.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-176">This option is available to support use cases where the meeting ID is known, such as when an application first creates the meeting, then retrieves meeting information later as a seperate action.</span></span>

#### <a name="request"></a><span data-ttu-id="8d3e0-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-177">Request</span></span>

<span data-ttu-id="8d3e0-178">В следующем запросе используется маркер пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-178">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2
```

<span data-ttu-id="8d3e0-179">В следующем запросе используется маркер приложения.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-179">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2
```

#### <a name="response"></a><span data-ttu-id="8d3e0-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-180">Response</span></span>

> <span data-ttu-id="8d3e0-181">**Примечание.** Показанный здесь объект отклика был сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-181">**Note:** The response object shown here has been shortened for readability.</span></span> <span data-ttu-id="8d3e0-182">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-182">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2",
    "creationDateTime": "2020-09-29T22:35:33.1594516Z",
    "startDateTime": "2020-09-29T22:35:31.389759Z",
    "endDateTime": "2020-09-29T23:35:31.389759Z",
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
    "subject": null,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    }
}
```

### <a name="example-3-retrieve-an-online-meeting-by-joinweburl"></a><span data-ttu-id="8d3e0-183">Пример 3. Извлечение собрания по сети с помощью JoinWebUrl</span><span class="sxs-lookup"><span data-stu-id="8d3e0-183">Example 3: Retrieve an online meeting by JoinWebUrl</span></span>
<span data-ttu-id="8d3e0-184">Сведения о собрании можно получить с помощью JoinWebUrl с помощью маркера пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-184">You can retrieve meeting information via JoinWebUrl by using either a user or application token.</span></span> <span data-ttu-id="8d3e0-185">Этот параметр доступен для поддержки случаев использования, когда ИД собрания неизвестен, но используется JoinWebUrl, например, когда пользователь создает собрание (например, в клиенте Microsoft Teams), и отдельное приложение должно получить сведения о собрании в качестве действия по последующему действию.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-185">This option is available to support use cases where the meeting ID is not known but the JoinWebUrl is, such as when a user creates a meeting (for example in the Microsoft Teams client), and a seperate application needs to retrieve meeting details as a followup action.</span></span>

#### <a name="request"></a><span data-ttu-id="8d3e0-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-186">Request</span></span>

<span data-ttu-id="8d3e0-187">В следующем запросе используется маркер пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-187">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

<span data-ttu-id="8d3e0-188">В следующем запросе используется маркер приложения.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-188">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

#### <a name="response"></a><span data-ttu-id="8d3e0-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-189">Response</span></span>

> <span data-ttu-id="8d3e0-190">**Примечание.** Показанный здесь объект отклика был сокращен для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-190">**Note:** The response object shown here has been shortened for readability.</span></span> <span data-ttu-id="8d3e0-191">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-191">All the properties will be returned from an actual call.</span></span>

```json
{
    "value": [
        {
            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2@thread.v2",
            "creationDateTime": "2020-09-29T22:35:33.1594516Z",
            "startDateTime": "2020-09-29T22:35:31.389759Z",
            "endDateTime": "2020-09-29T23:35:31.389759Z",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
            "subject": null,
            "autoAdmittedUsers": "EveryoneInCompany",
            "isEntryExitAnnounced": true,
            "allowedPresenters": "everyone",
            "videoTeleconferenceId": "(redacted)",
            "participants": {
                "organizer": {
                    "upn": "(redacted)",
                    "role": "presenter",
                    "identity": {
                        "user": {
                            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                            "displayName": null,
                            "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                            "identityProvider": "AAD"
                        }
                    }
                },
                "attendees": [],
                "producers": [],
                "contributors": []
            },
            "lobbyBypassSettings": {
                "scope": "organization",
                "isDialInBypassEnabled": false
            }
        }
    ]
}
```

### <a name="example-4-retrieve-the-attendee-report-of-a-live-event"></a><span data-ttu-id="8d3e0-192">Пример 4. Извлечение отчета участника о трансляции</span><span class="sxs-lookup"><span data-stu-id="8d3e0-192">Example 4: Retrieve the attendee report of a live event</span></span>
<span data-ttu-id="8d3e0-193">В следующем примере показан запрос на скачивание отчета участника.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-193">The following example shows a request to download an attendee report.</span></span>

#### <a name="request"></a><span data-ttu-id="8d3e0-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-194">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get-attendeeReport"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/attendeeReport
```

#### <a name="response"></a><span data-ttu-id="8d3e0-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-195">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/attendeeReport
```

### <a name="example-5-retrieve-the-recording-of-a-live-event"></a><span data-ttu-id="8d3e0-196">Пример 5. Извлечение записи трансляции</span><span class="sxs-lookup"><span data-stu-id="8d3e0-196">Example 5: Retrieve the recording of a live event</span></span>
<span data-ttu-id="8d3e0-197">В следующем примере показан запрос на скачивание записи.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-197">The following example shows a request to download a recording.</span></span>

#### <a name="request"></a><span data-ttu-id="8d3e0-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-198">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get-recording"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw@thread.v2/recording
```

#### <a name="response"></a><span data-ttu-id="8d3e0-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-199">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/recording
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
