---
title: Обновление onlineMeeting
description: Обновление свойств собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0781be9d2dcc289fe99aeb92f31f3e55ea273730
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241067"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="deb64-103">Обновление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="deb64-103">Update onlineMeeting</span></span>

<span data-ttu-id="deb64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb64-105">Обновление свойств указанного [объекта onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="deb64-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="deb64-106">См. [раздел Запрос](#request-body) тела для списка свойств, которые поддерживают обновление.</span><span class="sxs-lookup"><span data-stu-id="deb64-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb64-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deb64-107">Permissions</span></span>

| <span data-ttu-id="deb64-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb64-108">Permission type</span></span>                        | <span data-ttu-id="deb64-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb64-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="deb64-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb64-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="deb64-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deb64-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="deb64-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb64-113">Not Supported.</span></span>                              |
| <span data-ttu-id="deb64-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb64-114">Application</span></span>                            | <span data-ttu-id="deb64-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="deb64-115">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="deb64-116">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенное в политике, обновить онлайн-собрание от имени этого пользователя (пользовательский ID, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="deb64-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="deb64-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb64-117">HTTP request</span></span>
<span data-ttu-id="deb64-118">Обновление указанного onlineMeeting путем собрания ID с делегированным маркером:</span><span class="sxs-lookup"><span data-stu-id="deb64-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="deb64-119">Чтобы обновить указанный onlineMeeting, выдав ID с помощью маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="deb64-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="deb64-120">`userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="deb64-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="deb64-121">Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="deb64-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="deb64-122">`meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="deb64-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deb64-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deb64-123">Request headers</span></span>
| <span data-ttu-id="deb64-124">Имя</span><span class="sxs-lookup"><span data-stu-id="deb64-124">Name</span></span>          | <span data-ttu-id="deb64-125">Описание</span><span class="sxs-lookup"><span data-stu-id="deb64-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="deb64-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deb64-126">Authorization</span></span> | <span data-ttu-id="deb64-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb64-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="deb64-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deb64-129">Content-type</span></span>  | <span data-ttu-id="deb64-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb64-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb64-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deb64-132">Request body</span></span>
<span data-ttu-id="deb64-133">В таблице ниже перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="deb64-133">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="deb64-134">В орган запроса включаем только свойства, которые требуют обновления, за следующими исключениями:</span><span class="sxs-lookup"><span data-stu-id="deb64-134">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="deb64-135">Обновление даты начала или окончания собрания в Интернете всегда требует как **свойств startDateTime,** так и **endDateTime** в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="deb64-135">Updating the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="deb64-136">**Поле** организатора **свойства участников** не может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="deb64-136">**organizer** field of the **participants** property cannot be updated.</span></span> <span data-ttu-id="deb64-137">Организатор собрания не может быть изменен после создания собрания.</span><span class="sxs-lookup"><span data-stu-id="deb64-137">The organizer of the meeting cannot be modified once the meeting is created.</span></span>
- <span data-ttu-id="deb64-138">Обновление поля **участников** свойства **участников,** например добавление или удаление участника собрания, всегда требует полного списка участников в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="deb64-138">Updating the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="deb64-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb64-139">Property</span></span>             | <span data-ttu-id="deb64-140">Тип</span><span class="sxs-lookup"><span data-stu-id="deb64-140">Type</span></span>                                                         | <span data-ttu-id="deb64-141">Описание</span><span class="sxs-lookup"><span data-stu-id="deb64-141">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="deb64-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="deb64-142">startDateTime</span></span>        | <span data-ttu-id="deb64-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="deb64-143">DateTime</span></span>                                                     | <span data-ttu-id="deb64-144">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="deb64-144">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="deb64-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="deb64-145">endDateTime</span></span>          | <span data-ttu-id="deb64-146">DateTime</span><span class="sxs-lookup"><span data-stu-id="deb64-146">DateTime</span></span>                                                     | <span data-ttu-id="deb64-147">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="deb64-147">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="deb64-148">subject</span><span class="sxs-lookup"><span data-stu-id="deb64-148">subject</span></span>              | <span data-ttu-id="deb64-149">String</span><span class="sxs-lookup"><span data-stu-id="deb64-149">String</span></span>                                                       | <span data-ttu-id="deb64-150">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="deb64-150">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="deb64-151">participants</span><span class="sxs-lookup"><span data-stu-id="deb64-151">participants</span></span>         | [<span data-ttu-id="deb64-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="deb64-152">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="deb64-153">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="deb64-153">The participants associated with the online meeting.</span></span> <span data-ttu-id="deb64-154">Обновления могут быть только у участников.</span><span class="sxs-lookup"><span data-stu-id="deb64-154">Only attendees can be updated.</span></span>                                            |
| <span data-ttu-id="deb64-155">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="deb64-155">isEntryExitAnnounced</span></span> | <span data-ttu-id="deb64-156">Логический</span><span class="sxs-lookup"><span data-stu-id="deb64-156">Boolean</span></span>                                                      | <span data-ttu-id="deb64-157">Следует ли объявлять о том, когда звонители присоединяются или уходят.</span><span class="sxs-lookup"><span data-stu-id="deb64-157">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="deb64-158">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="deb64-158">lobbyBypassSettings</span></span>  | [<span data-ttu-id="deb64-159">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="deb64-159">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="deb64-160">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="deb64-160">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="deb64-161">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="deb64-161">allowedPresenters</span></span>    | <span data-ttu-id="deb64-162">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="deb64-162">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="deb64-163">Указывает, кто может быть презентовщиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="deb64-163">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="deb64-164">Возможные значения — это все, организация, roleIsPresenter, организатор и неизвестныйFutureValue.</span><span class="sxs-lookup"><span data-stu-id="deb64-164">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="deb64-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb64-165">Response</span></span>
<span data-ttu-id="deb64-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deb64-166">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deb64-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="deb64-167">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="deb64-168">Пример 1. Обновление startDateTime, endDateTime и субъекта</span><span class="sxs-lookup"><span data-stu-id="deb64-168">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="deb64-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb64-169">Request</span></span>

> <span data-ttu-id="deb64-170">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb64-170">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="deb64-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="deb64-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="deb64-172">C#</span><span class="sxs-lookup"><span data-stu-id="deb64-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deb64-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deb64-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deb64-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deb64-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deb64-175">Java</span><span class="sxs-lookup"><span data-stu-id="deb64-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="deb64-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb64-176">Response</span></span>

> <span data-ttu-id="deb64-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deb64-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="deb64-178">Пример 2. Обновление lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="deb64-178">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="deb64-179">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb64-179">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="deb64-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="deb64-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="deb64-181">C#</span><span class="sxs-lookup"><span data-stu-id="deb64-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deb64-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deb64-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deb64-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deb64-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deb64-184">Java</span><span class="sxs-lookup"><span data-stu-id="deb64-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="deb64-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb64-185">Response</span></span>

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


