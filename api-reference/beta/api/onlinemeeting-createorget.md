---
title: 'onlineMeeting: createOrGet'
description: Создайте онлайн-собрание с пользовательским внешним ИД. Если внешний ID уже существует, этот API возвращает объект onlineMeeting с этим внешним ИД.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 43cca80f5873e1349c8e057ded8270d710cfe632
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957844"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="e27a1-104">onlineMeeting: createOrGet</span><span class="sxs-lookup"><span data-stu-id="e27a1-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="e27a1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e27a1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e27a1-106">Создайте [объект onlineMeeting](../resources/onlinemeeting.md) с пользовательским внешним ИД.</span><span class="sxs-lookup"><span data-stu-id="e27a1-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="e27a1-107">Если внешний ID уже существует, этот API возвращает [объект onlineMeeting](../resources/onlinemeeting.md) с этим внешним ИД.</span><span class="sxs-lookup"><span data-stu-id="e27a1-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="e27a1-108">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="e27a1-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="e27a1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e27a1-109">Permissions</span></span>
<span data-ttu-id="e27a1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e27a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e27a1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e27a1-112">Permission type</span></span>                        | <span data-ttu-id="e27a1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e27a1-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e27a1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e27a1-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e27a1-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e27a1-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="e27a1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e27a1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e27a1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e27a1-117">Not Supported.</span></span>                              |
| <span data-ttu-id="e27a1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e27a1-118">Application</span></span>                            | <span data-ttu-id="e27a1-119">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="e27a1-119">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="e27a1-120">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенного в политике, создать или получить онлайн-встречу с внешним ИД от имени этого пользователя (пользовательский ID, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="e27a1-120">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to create or get an online meeting with external ID on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="e27a1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e27a1-121">HTTP request</span></span>
<span data-ttu-id="e27a1-122">Вызов **API createOrGet** с делегированным маркером:</span><span class="sxs-lookup"><span data-stu-id="e27a1-122">To call **createOrGet** API with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

<span data-ttu-id="e27a1-123">Вызов **API createOrGet** с помощью маркера приложения:</span><span class="sxs-lookup"><span data-stu-id="e27a1-123">To call **createOrGet** API with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> <span data-ttu-id="e27a1-124">**Примечание.** `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span><span class="sxs-lookup"><span data-stu-id="e27a1-124">**Note:** `userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="e27a1-125">Дополнительные сведения см. в статье [Политики доступа для приложений](/graph/cloud-communication-online-meeting-application-access-policy).</span><span class="sxs-lookup"><span data-stu-id="e27a1-125">See more details in [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e27a1-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e27a1-126">Request headers</span></span>
| <span data-ttu-id="e27a1-127">Имя</span><span class="sxs-lookup"><span data-stu-id="e27a1-127">Name</span></span>          | <span data-ttu-id="e27a1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e27a1-128">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="e27a1-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e27a1-129">Authorization</span></span> | <span data-ttu-id="e27a1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e27a1-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e27a1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e27a1-132">Content-type</span></span>  | <span data-ttu-id="e27a1-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e27a1-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e27a1-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e27a1-135">Request body</span></span>
<span data-ttu-id="e27a1-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e27a1-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e27a1-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="e27a1-137">Parameter</span></span>     | <span data-ttu-id="e27a1-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e27a1-138">Type</span></span>                                                       | <span data-ttu-id="e27a1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e27a1-139">Description</span></span>                                                                                          |
| :------------ | :--------------------------------------------------------- | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e27a1-140">chatInfo</span><span class="sxs-lookup"><span data-stu-id="e27a1-140">chatInfo</span></span>      | [<span data-ttu-id="e27a1-141">chatInfo</span><span class="sxs-lookup"><span data-stu-id="e27a1-141">chatInfo</span></span>](../resources/chatinfo.md)                       | <span data-ttu-id="e27a1-142">Сведения о чате, связанные с этой онлайн-встречей.</span><span class="sxs-lookup"><span data-stu-id="e27a1-142">The chat information associated with this online meeting.</span></span>                                            |
| <span data-ttu-id="e27a1-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e27a1-143">endDateTime</span></span>   | <span data-ttu-id="e27a1-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="e27a1-144">DateTime</span></span>                                                   | <span data-ttu-id="e27a1-145">Время окончания собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="e27a1-145">The meeting end time in UTC.</span></span>                                                                         |
| <span data-ttu-id="e27a1-146">externalId</span><span class="sxs-lookup"><span data-stu-id="e27a1-146">externalId</span></span>    | <span data-ttu-id="e27a1-147">String</span><span class="sxs-lookup"><span data-stu-id="e27a1-147">String</span></span>                                                     | <span data-ttu-id="e27a1-148">Внешний ID.</span><span class="sxs-lookup"><span data-stu-id="e27a1-148">The external ID.</span></span> <span data-ttu-id="e27a1-149">Пользовательский ID.</span><span class="sxs-lookup"><span data-stu-id="e27a1-149">A custom ID.</span></span> <span data-ttu-id="e27a1-150">(Обязательно)</span><span class="sxs-lookup"><span data-stu-id="e27a1-150">(Required)</span></span>                                                             |
| <span data-ttu-id="e27a1-151">participants</span><span class="sxs-lookup"><span data-stu-id="e27a1-151">participants</span></span>  | [<span data-ttu-id="e27a1-152">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="e27a1-152">meetingParticipants</span></span>](../resources/meetingparticipants.md) | <span data-ttu-id="e27a1-153">Участники, связанные с онлайн-собранием.</span><span class="sxs-lookup"><span data-stu-id="e27a1-153">The participants associated with the online meeting.</span></span>  <span data-ttu-id="e27a1-154">Это включает организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="e27a1-154">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="e27a1-155">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e27a1-155">startDateTime</span></span> | <span data-ttu-id="e27a1-156">DateTime</span><span class="sxs-lookup"><span data-stu-id="e27a1-156">DateTime</span></span>                                                   | <span data-ttu-id="e27a1-157">Время начала собрания в UTC.</span><span class="sxs-lookup"><span data-stu-id="e27a1-157">The meeting start time in UTC.</span></span>                                                                       |
| <span data-ttu-id="e27a1-158">subject</span><span class="sxs-lookup"><span data-stu-id="e27a1-158">subject</span></span>       | <span data-ttu-id="e27a1-159">String</span><span class="sxs-lookup"><span data-stu-id="e27a1-159">String</span></span>                                                     | <span data-ttu-id="e27a1-160">Тема собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="e27a1-160">The subject of the online meeting.</span></span>                                                                   |

> <span data-ttu-id="e27a1-161">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="e27a1-161">**Notes:**</span></span>
>
> - <span data-ttu-id="e27a1-162">Если **startDateTime** и **endDateTime** не предоставлены, по умолчанию **startDateTime** будет по умолчанию по текущему значению dateTime, а **значение endDateTime** равно **значению startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="e27a1-162">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="e27a1-163">Если **предоставляется startDateTime,** а **endDateTime** — нет, значение **endDateTime** будет равно **значению startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="e27a1-163">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="e27a1-164">Ошибка будет выброшена, если **endDateTime** предоставляется без **startDateTime** или если **endDateTime** является более ранним, чем **startDateTime.**</span><span class="sxs-lookup"><span data-stu-id="e27a1-164">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="e27a1-165">В **настоящее время chatInfo** поддерживается только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="e27a1-165">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="e27a1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27a1-166">Response</span></span>
<span data-ttu-id="e27a1-167">В случае успешной работы этот метод возвращает код ответа, если создается новое собрание, или код ответа при извлечении `201 Created` `200 OK` существующего собрания.</span><span class="sxs-lookup"><span data-stu-id="e27a1-167">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="e27a1-168">В обоих случаях [объект onlineMeeting](../resources/onlinemeeting.md) возвращается в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e27a1-168">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e27a1-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="e27a1-169">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="e27a1-170">Пример 1. Создание или создание собрания в Интернете с внешним ИД</span><span class="sxs-lookup"><span data-stu-id="e27a1-170">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="e27a1-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27a1-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e27a1-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="e27a1-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting-1"
}-->

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "subject": "Create a meeting with customId provided",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "role": "presenter",
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="e27a1-173">C#</span><span class="sxs-lookup"><span data-stu-id="e27a1-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e27a1-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e27a1-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e27a1-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e27a1-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e27a1-176">Java</span><span class="sxs-lookup"><span data-stu-id="e27a1-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e27a1-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27a1-177">Response</span></span>

><span data-ttu-id="e27a1-178">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e27a1-178">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "0",
        "replyChainMessageId": null
    },
}
```


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="e27a1-179">Пример 2. Создание или участие в онлайн-собрании в канале Microsoft Teams с внешним ИД</span><span class="sxs-lookup"><span data-stu-id="e27a1-179">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="e27a1-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="e27a1-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e27a1-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="e27a1-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting-2"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2"
    },
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "upn": "test1@contoso.com"
            }
        ]
    },
    "subject": "Create a meeting with customId provided"
}
```
# <a name="c"></a>[<span data-ttu-id="e27a1-182">C#</span><span class="sxs-lookup"><span data-stu-id="e27a1-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e27a1-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e27a1-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e27a1-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e27a1-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e27a1-185">Java</span><span class="sxs-lookup"><span data-stu-id="e27a1-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e27a1-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="e27a1-186">Response</span></span>

><span data-ttu-id="e27a1-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e27a1-187">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "1599805818399",
        "replyChainMessageId": null
    },
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


