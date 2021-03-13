---
title: Обновление onlineMeeting
description: Обновление свойств собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 14d083bb6ed6e74fe1017ab4a7a87ed2bf159cc9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775607"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="2d159-103">Обновление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="2d159-103">Update onlineMeeting</span></span>

<span data-ttu-id="2d159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d159-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d159-105">Обновление свойств указанного [объекта onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="2d159-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="2d159-106">См. [раздел Запрос](#request-body) тела для списка свойств, которые поддерживают обновление.</span><span class="sxs-lookup"><span data-stu-id="2d159-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d159-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d159-107">Permissions</span></span>

| <span data-ttu-id="2d159-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d159-108">Permission type</span></span>                        | <span data-ttu-id="2d159-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d159-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2d159-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d159-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d159-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d159-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="2d159-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d159-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d159-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d159-113">Not Supported.</span></span>                              |
| <span data-ttu-id="2d159-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d159-114">Application</span></span>                            | <span data-ttu-id="2d159-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="2d159-115">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="2d159-116">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенное в политике, обновить онлайн-собрание от имени этого пользователя (пользовательский ID, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="2d159-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="2d159-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d159-117">HTTP request</span></span>
<span data-ttu-id="2d159-118">Обновление указанного onlineMeeting путем собрания ID с делегированным маркером:</span><span class="sxs-lookup"><span data-stu-id="2d159-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="2d159-119">Чтобы обновить указанный onlineMeeting, выдав ID с помощью маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="2d159-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="2d159-120">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="2d159-120">**Notes:**</span></span>
> - <span data-ttu-id="2d159-121">`userId`— это объектный ID пользователя на портале [управления пользователями Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="2d159-121">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="2d159-122">Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="2d159-122">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="2d159-123">`meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="2d159-123">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d159-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d159-124">Request headers</span></span>
| <span data-ttu-id="2d159-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2d159-125">Name</span></span>          | <span data-ttu-id="2d159-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2d159-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="2d159-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d159-127">Authorization</span></span> | <span data-ttu-id="2d159-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d159-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2d159-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d159-130">Content-type</span></span>  | <span data-ttu-id="2d159-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d159-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d159-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d159-133">Request body</span></span>
<span data-ttu-id="2d159-134">В таблице ниже перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="2d159-134">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="2d159-135">В орган запроса включаем только свойства, которые требуют обновления, за следующими исключениями:</span><span class="sxs-lookup"><span data-stu-id="2d159-135">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="2d159-136">Для настройки даты начала или окончания собрания в интернете всегда требуются свойства **startDateTime** и **endDateTime** в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="2d159-136">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="2d159-137">Для настройки **поля** участников  свойства участников, например добавления или удаления участника собрания, всегда требуется полный список участников в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="2d159-137">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="2d159-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d159-138">Property</span></span>             | <span data-ttu-id="2d159-139">Тип</span><span class="sxs-lookup"><span data-stu-id="2d159-139">Type</span></span>                                                         | <span data-ttu-id="2d159-140">Описание</span><span class="sxs-lookup"><span data-stu-id="2d159-140">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2d159-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2d159-141">startDateTime</span></span>        | <span data-ttu-id="2d159-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d159-142">DateTime</span></span>                                                     | <span data-ttu-id="2d159-143">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="2d159-143">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="2d159-144">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2d159-144">endDateTime</span></span>          | <span data-ttu-id="2d159-145">DateTime</span><span class="sxs-lookup"><span data-stu-id="2d159-145">DateTime</span></span>                                                     | <span data-ttu-id="2d159-146">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="2d159-146">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="2d159-147">subject</span><span class="sxs-lookup"><span data-stu-id="2d159-147">subject</span></span>              | <span data-ttu-id="2d159-148">String</span><span class="sxs-lookup"><span data-stu-id="2d159-148">String</span></span>                                                       | <span data-ttu-id="2d159-149">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="2d159-149">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="2d159-150">participants</span><span class="sxs-lookup"><span data-stu-id="2d159-150">participants</span></span>         | [<span data-ttu-id="2d159-151">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="2d159-151">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="2d159-152">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="2d159-152">The participants associated with the online meeting.</span></span> <span data-ttu-id="2d159-153">Это включает организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="2d159-153">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="2d159-154">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="2d159-154">isEntryExitAnnounced</span></span> | <span data-ttu-id="2d159-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d159-155">Boolean</span></span>                                                      | <span data-ttu-id="2d159-156">Следует ли объявлять о том, когда звонители присоединяются или уходят.</span><span class="sxs-lookup"><span data-stu-id="2d159-156">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="2d159-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="2d159-157">lobbyBypassSettings</span></span>  | [<span data-ttu-id="2d159-158">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="2d159-158">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="2d159-159">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="2d159-159">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="2d159-160">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="2d159-160">allowedPresenters</span></span>    | <span data-ttu-id="2d159-161">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="2d159-161">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="2d159-162">Указывает, кто может быть презентовщиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="2d159-162">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="2d159-163">Возможные значения — это все, организация, roleIsPresenter, организатор и неизвестныйFutureValue.</span><span class="sxs-lookup"><span data-stu-id="2d159-163">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="2d159-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d159-164">Response</span></span>
<span data-ttu-id="2d159-165">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d159-165">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d159-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d159-166">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="2d159-167">Пример 1. Обновление startDateTime, endDateTime и субъекта</span><span class="sxs-lookup"><span data-stu-id="2d159-167">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="2d159-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d159-168">Request</span></span>

> <span data-ttu-id="2d159-169">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d159-169">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d159-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d159-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="2d159-171">C#</span><span class="sxs-lookup"><span data-stu-id="2d159-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d159-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d159-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d159-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d159-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d159-174">Java</span><span class="sxs-lookup"><span data-stu-id="2d159-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d159-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d159-175">Response</span></span>

> <span data-ttu-id="2d159-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d159-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="2d159-178">Пример 2. Обновление lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="2d159-178">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="2d159-179">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d159-179">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="2d159-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d159-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2d159-181">C#</span><span class="sxs-lookup"><span data-stu-id="2d159-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d159-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d159-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d159-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d159-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d159-184">Java</span><span class="sxs-lookup"><span data-stu-id="2d159-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d159-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d159-185">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
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
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


