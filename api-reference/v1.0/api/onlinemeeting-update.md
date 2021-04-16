---
title: Обновление onlineMeeting
description: Обновление свойств собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 42bc40f6dc1ec6f72996ade9b0a552bc94d0a69f
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870011"
---
# <a name="update-onlinemeeting"></a><span data-ttu-id="aaab9-103">Обновление onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="aaab9-103">Update onlineMeeting</span></span>

<span data-ttu-id="aaab9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaab9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aaab9-105">Обновление свойств указанного [объекта onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="aaab9-105">Update the properties of the specified [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

<span data-ttu-id="aaab9-106">См. [раздел Запрос](#request-body) тела для списка свойств, которые поддерживают обновление.</span><span class="sxs-lookup"><span data-stu-id="aaab9-106">Please see [Request body](#request-body) section for the list of properties that support updating.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaab9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaab9-107">Permissions</span></span>

| <span data-ttu-id="aaab9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaab9-108">Permission type</span></span>                        | <span data-ttu-id="aaab9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaab9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="aaab9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaab9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aaab9-111">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaab9-111">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="aaab9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaab9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaab9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaab9-113">Not Supported.</span></span>                              |
| <span data-ttu-id="aaab9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaab9-114">Application</span></span>                            | <span data-ttu-id="aaab9-115">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="aaab9-115">OnlineMeetings.ReadWrite.All\*</span></span>               |

> [!IMPORTANT]
> <span data-ttu-id="aaab9-116">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенное в политике, обновить онлайн-собрание от имени этого пользователя (пользовательский ID, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="aaab9-116">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to update an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="aaab9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaab9-117">HTTP request</span></span>
<span data-ttu-id="aaab9-118">Обновление указанного onlineMeeting путем собрания ID с делегированным маркером:</span><span class="sxs-lookup"><span data-stu-id="aaab9-118">To update the specified onlineMeeting by meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="aaab9-119">Чтобы обновить указанный onlineMeeting, выдав ID с помощью маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="aaab9-119">To update the specified onlineMeeting by meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - <span data-ttu-id="aaab9-120">`userId`— это объектный ID пользователя на портале [управления пользователями Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="aaab9-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="aaab9-121">Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="aaab9-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="aaab9-122">`meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="aaab9-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaab9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaab9-123">Request headers</span></span>
| <span data-ttu-id="aaab9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="aaab9-124">Name</span></span>          | <span data-ttu-id="aaab9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="aaab9-125">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="aaab9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaab9-126">Authorization</span></span> | <span data-ttu-id="aaab9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaab9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="aaab9-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaab9-129">Content-type</span></span>  | <span data-ttu-id="aaab9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaab9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaab9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaab9-132">Request body</span></span>
<span data-ttu-id="aaab9-133">В таблице ниже перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="aaab9-133">The table below lists the properties that can be updated.</span></span> <span data-ttu-id="aaab9-134">В орган запроса включаем только свойства, которые требуют обновления, за следующими исключениями:</span><span class="sxs-lookup"><span data-stu-id="aaab9-134">In the request body, include only the properties that need updating, with the following exceptions:</span></span>

- <span data-ttu-id="aaab9-135">Для настройки даты начала или окончания собрания в интернете всегда требуются свойства **startDateTime** и **endDateTime** в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="aaab9-135">Adjusting the start or end date/time of an online meeting always requires both **startDateTime** and **endDateTime** properties in the request body.</span></span>
- <span data-ttu-id="aaab9-136">Для настройки **поля** участников  свойства участников, например добавления или удаления участника собрания, всегда требуется полный список участников в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="aaab9-136">Adjusting the **attendees** field of the **participants** property, such as adding or removing an attendee to the meeting, always requires the full list of attendees in the request body.</span></span>

| <span data-ttu-id="aaab9-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaab9-137">Property</span></span>             | <span data-ttu-id="aaab9-138">Тип</span><span class="sxs-lookup"><span data-stu-id="aaab9-138">Type</span></span>                                                         | <span data-ttu-id="aaab9-139">Описание</span><span class="sxs-lookup"><span data-stu-id="aaab9-139">Description</span></span>                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aaab9-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aaab9-140">startDateTime</span></span>        | <span data-ttu-id="aaab9-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="aaab9-141">DateTime</span></span>                                                     | <span data-ttu-id="aaab9-142">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="aaab9-142">The meeting start time in UTC.</span></span>                                                                                                                 |
| <span data-ttu-id="aaab9-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="aaab9-143">endDateTime</span></span>          | <span data-ttu-id="aaab9-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="aaab9-144">DateTime</span></span>                                                     | <span data-ttu-id="aaab9-145">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="aaab9-145">The meeting end time in UTC.</span></span>                                                                                                                   |
| <span data-ttu-id="aaab9-146">subject</span><span class="sxs-lookup"><span data-stu-id="aaab9-146">subject</span></span>              | <span data-ttu-id="aaab9-147">String</span><span class="sxs-lookup"><span data-stu-id="aaab9-147">String</span></span>                                                       | <span data-ttu-id="aaab9-148">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="aaab9-148">The subject of the online meeting.</span></span>                                                                                                             |
| <span data-ttu-id="aaab9-149">participants</span><span class="sxs-lookup"><span data-stu-id="aaab9-149">participants</span></span>         | [<span data-ttu-id="aaab9-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="aaab9-150">meetingParticipants</span></span>](../resources/meetingparticipants.md)   | <span data-ttu-id="aaab9-151">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="aaab9-151">The participants associated with the online meeting.</span></span> <span data-ttu-id="aaab9-152">Это включает организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="aaab9-152">This includes the organizer and the attendees.</span></span>                                            |
| <span data-ttu-id="aaab9-153">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="aaab9-153">isEntryExitAnnounced</span></span> | <span data-ttu-id="aaab9-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaab9-154">Boolean</span></span>                                                      | <span data-ttu-id="aaab9-155">Следует ли объявлять о том, когда звонители присоединяются или уходят.</span><span class="sxs-lookup"><span data-stu-id="aaab9-155">Whether or not to announce when callers join or leave.</span></span>                                                                                         |
| <span data-ttu-id="aaab9-156">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="aaab9-156">lobbyBypassSettings</span></span>  | [<span data-ttu-id="aaab9-157">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="aaab9-157">lobbyBypassSettings</span></span>](../resources/lobbyBypassSettings.md)   | <span data-ttu-id="aaab9-158">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="aaab9-158">Specifies which participants can bypass the meeting lobby.</span></span>                                                                                     |
| <span data-ttu-id="aaab9-159">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="aaab9-159">allowedPresenters</span></span>    | <span data-ttu-id="aaab9-160">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="aaab9-160">onlineMeetingPresenters</span></span>                                      | <span data-ttu-id="aaab9-161">Указывает, кто может быть презентовщиком на собрании.</span><span class="sxs-lookup"><span data-stu-id="aaab9-161">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="aaab9-162">Возможные значения — это все, организация, roleIsPresenter, организатор и неизвестныйFutureValue.</span><span class="sxs-lookup"><span data-stu-id="aaab9-162">Possible values are everyone, organization, roleIsPresenter, organizer, and unknownFutureValue.</span></span> |

## <a name="response"></a><span data-ttu-id="aaab9-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaab9-163">Response</span></span>
<span data-ttu-id="aaab9-164">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaab9-164">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aaab9-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="aaab9-165">Examples</span></span>

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a><span data-ttu-id="aaab9-166">Пример 1. Обновление startDateTime, endDateTime и субъекта</span><span class="sxs-lookup"><span data-stu-id="aaab9-166">Example 1: Update the startDateTime, endDateTime and subject</span></span>

#### <a name="request"></a><span data-ttu-id="aaab9-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaab9-167">Request</span></span>

> <span data-ttu-id="aaab9-168">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="aaab9-168">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="aaab9-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaab9-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[<span data-ttu-id="aaab9-170">C#</span><span class="sxs-lookup"><span data-stu-id="aaab9-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaab9-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaab9-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaab9-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaab9-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaab9-173">Java</span><span class="sxs-lookup"><span data-stu-id="aaab9-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aaab9-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaab9-174">Response</span></span>

> <span data-ttu-id="aaab9-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaab9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="example-2-update-the-lobbybypasssettings"></a><span data-ttu-id="aaab9-177">Пример 2. Обновление lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="aaab9-177">Example 2: Update the lobbyBypassSettings</span></span>
> <span data-ttu-id="aaab9-178">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="aaab9-178">**Note:** The meeting ID has been truncated for readability.</span></span>


# <a name="http"></a>[<span data-ttu-id="aaab9-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaab9-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="aaab9-180">C#</span><span class="sxs-lookup"><span data-stu-id="aaab9-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaab9-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaab9-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaab9-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaab9-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaab9-183">Java</span><span class="sxs-lookup"><span data-stu-id="aaab9-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aaab9-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaab9-184">Response</span></span>

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


