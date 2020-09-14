---
title: 'Онлинемитинг: Креатеоржет'
description: Создайте собрание по сети с настраиваемым указанным внешним ИДЕНТИФИКАТОРом. Если внешний идентификатор уже существует, этот API возвратит объект **онлинемитинг** с этим внешним идентификатором.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d99a9ac98fd5fbb4ca5c96904831bb76c93b158c
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651325"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="f37a7-104">Онлинемитинг: Креатеоржет</span><span class="sxs-lookup"><span data-stu-id="f37a7-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="f37a7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f37a7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f37a7-106">Создание объекта [онлинемитинг](../resources/onlinemeeting.md) с настраиваемым указанным внешним идентификатором.</span><span class="sxs-lookup"><span data-stu-id="f37a7-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="f37a7-107">Если внешний идентификатор уже существует, этот API возвратит объект [онлинемитинг](../resources/onlinemeeting.md) с этим внешним идентификатором.</span><span class="sxs-lookup"><span data-stu-id="f37a7-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="f37a7-108">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="f37a7-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="f37a7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f37a7-109">Permissions</span></span>
<span data-ttu-id="f37a7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f37a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f37a7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f37a7-112">Permission type</span></span>                        | <span data-ttu-id="f37a7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f37a7-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f37a7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f37a7-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f37a7-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f37a7-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="f37a7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f37a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f37a7-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f37a7-117">Not Supported</span></span>                               |
| <span data-ttu-id="f37a7-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="f37a7-118">Application</span></span>                            | <span data-ttu-id="f37a7-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="f37a7-119">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="f37a7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f37a7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="f37a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f37a7-121">Request headers</span></span>
| <span data-ttu-id="f37a7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f37a7-122">Name</span></span>          | <span data-ttu-id="f37a7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f37a7-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f37a7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f37a7-124">Authorization</span></span> | <span data-ttu-id="f37a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f37a7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f37a7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f37a7-127">Content-type</span></span>  | <span data-ttu-id="f37a7-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f37a7-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f37a7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f37a7-130">Request body</span></span>
<span data-ttu-id="f37a7-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f37a7-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f37a7-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="f37a7-132">Parameter</span></span>        | <span data-ttu-id="f37a7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f37a7-133">Type</span></span>                                     |<span data-ttu-id="f37a7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f37a7-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="f37a7-135">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f37a7-135">chatInfo</span></span>         |[<span data-ttu-id="f37a7-136">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f37a7-136">chatInfo</span></span>](../resources/chatinfo.md)                   |<span data-ttu-id="f37a7-137">Сведения о чате, связанные с этим собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="f37a7-137">The chat information associated with this online meeting.</span></span>|
| <span data-ttu-id="f37a7-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f37a7-138">endDateTime</span></span>      | <span data-ttu-id="f37a7-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="f37a7-139">DateTime</span></span>                                 | <span data-ttu-id="f37a7-140">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f37a7-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="f37a7-141">externalId</span><span class="sxs-lookup"><span data-stu-id="f37a7-141">externalId</span></span>       | <span data-ttu-id="f37a7-142">String</span><span class="sxs-lookup"><span data-stu-id="f37a7-142">String</span></span>                                   | <span data-ttu-id="f37a7-143">Внешний идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f37a7-143">The external ID.</span></span> <span data-ttu-id="f37a7-144">Настраиваемый идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f37a7-144">A custom ID.</span></span> <span data-ttu-id="f37a7-145">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="f37a7-145">(Required)</span></span> |
| <span data-ttu-id="f37a7-146">participants</span><span class="sxs-lookup"><span data-stu-id="f37a7-146">participants</span></span>     | [<span data-ttu-id="f37a7-147">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="f37a7-147">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="f37a7-148">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="f37a7-148">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f37a7-149">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="f37a7-149">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f37a7-150">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f37a7-150">startDateTime</span></span>    | <span data-ttu-id="f37a7-151">DateTime</span><span class="sxs-lookup"><span data-stu-id="f37a7-151">DateTime</span></span>                                 | <span data-ttu-id="f37a7-152">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f37a7-152">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="f37a7-153">subject</span><span class="sxs-lookup"><span data-stu-id="f37a7-153">subject</span></span>          | <span data-ttu-id="f37a7-154">String</span><span class="sxs-lookup"><span data-stu-id="f37a7-154">String</span></span>                                   | <span data-ttu-id="f37a7-155">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="f37a7-155">The subject of the online meeting.</span></span> |

> <span data-ttu-id="f37a7-156">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="f37a7-156">**Notes:**</span></span>
>
> - <span data-ttu-id="f37a7-157">Если **startDateTime** и **endDateTime** не указаны, то **startDateTime** по умолчанию будет иметь текущее значение DateTime, а значение **endDateTime** будет равно **startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="f37a7-157">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f37a7-158">Если предоставлено значение **startDateTime** , но значение **endDateTime** не задано, значение **endDateTime** будет равно **startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="f37a7-158">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="f37a7-159">Если **endDateTime** предоставляется без **startDateTime** или **endDateTime** более ранней версии, чем **startDateTime**, будет выдаваться сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f37a7-159">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>
>
> - <span data-ttu-id="f37a7-160">В настоящее время **чатинфо** поддерживается только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="f37a7-160">Currently **chatInfo** is only supported in beta.</span></span>

## <a name="response"></a><span data-ttu-id="f37a7-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f37a7-161">Response</span></span>
<span data-ttu-id="f37a7-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если создается новое собрание, или `200 OK` код ответа при получении существующего собрания.</span><span class="sxs-lookup"><span data-stu-id="f37a7-162">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="f37a7-163">В обоих случаях объект [онлинемитинг](../resources/onlinemeeting.md) возвращается в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f37a7-163">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f37a7-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="f37a7-164">Examples</span></span>

### <a name="example-1-create-or-get-an-online-meeting-with-an-external-id"></a><span data-ttu-id="f37a7-165">Пример 1: создание или получение собрания по сети с внешним ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="f37a7-165">Example 1: Create or get an online meeting with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="f37a7-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f37a7-166">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
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
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```

#### <a name="response"></a><span data-ttu-id="f37a7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="f37a7-167">Response</span></span>

><span data-ttu-id="f37a7-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f37a7-168">**Note:** The response object shown here might be shortened for readability.</span></span> 

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


### <a name="example-2-create-or-get-an-online-meeting-in-a-microsoft-teams-channel-with-an-external-id"></a><span data-ttu-id="f37a7-169">Пример 2: создание или получение собрания по сети в канале Microsoft Teams с внешним ИДЕНТИФИКАТОРом</span><span class="sxs-lookup"><span data-stu-id="f37a7-169">Example 2: Create or get an online meeting in a Microsoft Teams channel with an external ID</span></span>

#### <a name="request"></a><span data-ttu-id="f37a7-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="f37a7-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
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

#### <a name="response"></a><span data-ttu-id="f37a7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="f37a7-171">Response</span></span>

><span data-ttu-id="f37a7-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f37a7-172">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
