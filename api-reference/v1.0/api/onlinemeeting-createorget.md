---
title: 'Онлинемитинг: Креатеоржет'
description: Создайте собрание по сети с настраиваемым указанным внешним ИДЕНТИФИКАТОРом. Если внешний идентификатор уже существует, этот API возвратит объект **онлинемитинг** с этим внешним идентификатором.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dfb4d697df9d49f177510097ffa5dddfe255f12a
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842822"
---
# <a name="onlinemeeting-createorget"></a><span data-ttu-id="144a9-104">Онлинемитинг: Креатеоржет</span><span class="sxs-lookup"><span data-stu-id="144a9-104">onlineMeeting: createOrGet</span></span>

<span data-ttu-id="144a9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="144a9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="144a9-106">Создание объекта [онлинемитинг](../resources/onlinemeeting.md) с настраиваемым указанным внешним идентификатором.</span><span class="sxs-lookup"><span data-stu-id="144a9-106">Create an [onlineMeeting](../resources/onlinemeeting.md) object with a custom specified external ID.</span></span> <span data-ttu-id="144a9-107">Если внешний идентификатор уже существует, этот API возвратит объект [онлинемитинг](../resources/onlinemeeting.md) с этим внешним идентификатором.</span><span class="sxs-lookup"><span data-stu-id="144a9-107">If the external ID already exists, this API will return the [onlineMeeting](../resources/onlinemeeting.md) object with that external ID.</span></span> 

> <span data-ttu-id="144a9-108">**Примечание.** Собрание не отображается в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="144a9-108">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="144a9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="144a9-109">Permissions</span></span>
<span data-ttu-id="144a9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="144a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="144a9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="144a9-112">Permission type</span></span>                        | <span data-ttu-id="144a9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="144a9-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="144a9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="144a9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="144a9-115">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="144a9-115">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="144a9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="144a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144a9-117">Not supported.</span></span>                               |
| <span data-ttu-id="144a9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="144a9-118">Application</span></span>                            | <span data-ttu-id="144a9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144a9-119">Not supported.</span></span>                |

## <a name="http-request"></a><span data-ttu-id="144a9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="144a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

## <a name="request-headers"></a><span data-ttu-id="144a9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="144a9-121">Request headers</span></span>
| <span data-ttu-id="144a9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="144a9-122">Name</span></span>          | <span data-ttu-id="144a9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="144a9-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="144a9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="144a9-124">Authorization</span></span> | <span data-ttu-id="144a9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="144a9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="144a9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="144a9-127">Content-type</span></span>  | <span data-ttu-id="144a9-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="144a9-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="144a9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="144a9-130">Request body</span></span>
<span data-ttu-id="144a9-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="144a9-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="144a9-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="144a9-132">Parameter</span></span>        | <span data-ttu-id="144a9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="144a9-133">Type</span></span>                                     |<span data-ttu-id="144a9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="144a9-134">Description</span></span>                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| <span data-ttu-id="144a9-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="144a9-135">endDateTime</span></span>      | <span data-ttu-id="144a9-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="144a9-136">DateTime</span></span>                                 | <span data-ttu-id="144a9-137">Время окончания собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="144a9-137">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="144a9-138">externalId</span><span class="sxs-lookup"><span data-stu-id="144a9-138">externalId</span></span>       | <span data-ttu-id="144a9-139">String</span><span class="sxs-lookup"><span data-stu-id="144a9-139">String</span></span>                                   | <span data-ttu-id="144a9-140">Внешний идентификатор.</span><span class="sxs-lookup"><span data-stu-id="144a9-140">The external ID.</span></span> <span data-ttu-id="144a9-141">Настраиваемый идентификатор.</span><span class="sxs-lookup"><span data-stu-id="144a9-141">A custom ID.</span></span> <span data-ttu-id="144a9-142">Потребоваться</span><span class="sxs-lookup"><span data-stu-id="144a9-142">(Required)</span></span> |
| <span data-ttu-id="144a9-143">participants</span><span class="sxs-lookup"><span data-stu-id="144a9-143">participants</span></span>     | [<span data-ttu-id="144a9-144">митингпартиЦипантс</span><span class="sxs-lookup"><span data-stu-id="144a9-144">meetingParticipants</span></span>](../resources/meetingparticipants.md)          | <span data-ttu-id="144a9-145">Участники, связанные с собранием по сети.</span><span class="sxs-lookup"><span data-stu-id="144a9-145">The participants associated with the online meeting.</span></span>  <span data-ttu-id="144a9-146">Сюда входят Организатор и участники.</span><span class="sxs-lookup"><span data-stu-id="144a9-146">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="144a9-147">startDateTime</span><span class="sxs-lookup"><span data-stu-id="144a9-147">startDateTime</span></span>    | <span data-ttu-id="144a9-148">DateTime</span><span class="sxs-lookup"><span data-stu-id="144a9-148">DateTime</span></span>                                 | <span data-ttu-id="144a9-149">Время начала собрания в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="144a9-149">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="144a9-150">subject</span><span class="sxs-lookup"><span data-stu-id="144a9-150">subject</span></span>          | <span data-ttu-id="144a9-151">String</span><span class="sxs-lookup"><span data-stu-id="144a9-151">String</span></span>                                   | <span data-ttu-id="144a9-152">Тема собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="144a9-152">The subject of the online meeting.</span></span> |

> <span data-ttu-id="144a9-153">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="144a9-153">**Notes:**</span></span>
>
> - <span data-ttu-id="144a9-154">Если **startDateTime** и **endDateTime** не указаны, то **startDateTime** по умолчанию будет иметь текущее значение DateTime, а значение **endDateTime** будет равно **startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="144a9-154">If the **startDateTime** and **endDateTime** are not provided, the **startDateTime** will default to the current dateTime value and **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="144a9-155">Если предоставлено значение **startDateTime** , но значение **endDateTime** не задано, значение **endDateTime** будет равно **startDateTime** + 1 час.</span><span class="sxs-lookup"><span data-stu-id="144a9-155">If the **startDateTime** is provided, but **endDateTime** is not, the **endDateTime** value will equal the **startDateTime** + 1 hour.</span></span>
>
> - <span data-ttu-id="144a9-156">Если **endDateTime** предоставляется без **startDateTime** или **endDateTime** более ранней версии, чем **startDateTime**, будет выдаваться сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="144a9-156">An error will be thrown if the **endDateTime** is provided without the **startDateTime** or if the **endDateTime** is earlier than the **startDateTime**.</span></span>

## <a name="response"></a><span data-ttu-id="144a9-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="144a9-157">Response</span></span>
<span data-ttu-id="144a9-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если создается новое собрание, или `200 OK` код ответа при получении существующего собрания.</span><span class="sxs-lookup"><span data-stu-id="144a9-158">If successful, this method returns a `201 Created` response code if a new meeting is created, or a `200 OK` response code if an existing meeting is retrieved.</span></span> <span data-ttu-id="144a9-159">В обоих случаях объект [онлинемитинг](../resources/onlinemeeting.md) возвращается в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="144a9-159">In both cases, an [onlineMeeting](../resources/onlinemeeting.md) object is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="144a9-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="144a9-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="144a9-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="144a9-161">Request</span></span>

<span data-ttu-id="144a9-162">В приведенном ниже примере показано, как создать или получить собрание по сети с внешним ИДЕНТИФИКАТОРом.</span><span class="sxs-lookup"><span data-stu-id="144a9-162">The following example shows how to create or get an online meeting with an external ID.</span></span>


# <a name="http"></a>[<span data-ttu-id="144a9-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="144a9-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings/createOrGet
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
# <a name="c"></a>[<span data-ttu-id="144a9-164">C#</span><span class="sxs-lookup"><span data-stu-id="144a9-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="144a9-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="144a9-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="144a9-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="144a9-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="144a9-167">Java</span><span class="sxs-lookup"><span data-stu-id="144a9-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="144a9-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="144a9-168">Response</span></span>

><span data-ttu-id="144a9-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="144a9-169">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
