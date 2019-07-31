---
title: Получение вызова
description: Получение свойств и связей объекта Call.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9c6807250e66947605cd7abb990a7646301af8a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944544"
---
# <a name="get-call"></a><span data-ttu-id="02462-103">Получение вызова</span><span class="sxs-lookup"><span data-stu-id="02462-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02462-104">Получение свойств и связей объекта Call.</span><span class="sxs-lookup"><span data-stu-id="02462-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02462-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02462-105">Permissions</span></span>
<span data-ttu-id="02462-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02462-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02462-108">Permission type</span></span> | <span data-ttu-id="02462-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02462-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="02462-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02462-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02462-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02462-111">Not Supported.</span></span>                         |
| <span data-ttu-id="02462-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02462-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02462-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02462-113">Not Supported.</span></span>                         |
| <span data-ttu-id="02462-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="02462-114">Application</span></span>                            | <span data-ttu-id="02462-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="02462-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="02462-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02462-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02462-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02462-117">Optional query parameters</span></span>
<span data-ttu-id="02462-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="02462-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02462-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02462-119">Request headers</span></span>
| <span data-ttu-id="02462-120">Имя</span><span class="sxs-lookup"><span data-stu-id="02462-120">Name</span></span>          | <span data-ttu-id="02462-121">Описание</span><span class="sxs-lookup"><span data-stu-id="02462-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="02462-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02462-122">Authorization</span></span> | <span data-ttu-id="02462-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02462-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02462-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02462-125">Request body</span></span>
<span data-ttu-id="02462-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02462-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02462-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="02462-127">Response</span></span>
<span data-ttu-id="02462-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Call](../resources/call.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02462-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02462-129">Пример</span><span class="sxs-lookup"><span data-stu-id="02462-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02462-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="02462-130">Request</span></span>
<span data-ttu-id="02462-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02462-131">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="02462-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="02462-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02462-133">C#</span><span class="sxs-lookup"><span data-stu-id="02462-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02462-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="02462-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02462-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="02462-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="02462-136">Java</span><span class="sxs-lookup"><span data-stu-id="02462-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="02462-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="02462-137">Response</span></span>

> <span data-ttu-id="02462-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02462-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2821

{
  "activeModalities": [
    "unknown"
  ],
  "answeredBy": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "callRoutes": [
    {
      "final": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "original": {
        "phone": {
          "id": "+14258828080"
        }
      },
      "routingType": "forwarded"
    }
  ],
  "callbackUri": "callbackUri-value",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "direction": "incoming",
  "id": "id-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "meetingCapability": {
    "allowAnonymousUsersToDialOut": true,
    "allowAnonymousUsersToStartMeeting": true,
    "autoAdmittedUsers": "everyoneInCompany"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "myParticipantId-value",
  "requestedModalities": [
    "audio", "video"
  ],
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": [
    "none"
  ],
  "source": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "state": "incoming",
  "subject": "subject-value",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    }
  ],
  "tenantId": "tenantId-value",
  "terminationReason": "terminationReason-value",
  "toneInfo": {
    "sequenceId": 99,
    "tone": "tone0"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
