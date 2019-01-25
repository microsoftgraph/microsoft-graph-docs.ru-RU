---
title: Начало звонка
description: Извлечение свойств и связи объекта вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f5f530fac12ae61c47a5a5e3e0f900720aac4c4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530071"
---
# <a name="get-call"></a><span data-ttu-id="a0d50-103">Начало звонка</span><span class="sxs-lookup"><span data-stu-id="a0d50-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d50-104">Извлечение свойств и связи объекта вызова.</span><span class="sxs-lookup"><span data-stu-id="a0d50-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d50-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d50-105">Permissions</span></span>
<span data-ttu-id="a0d50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0d50-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0d50-108">Permission type</span></span> | <span data-ttu-id="a0d50-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0d50-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="a0d50-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0d50-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0d50-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d50-111">Not Supported.</span></span>                         |
| <span data-ttu-id="a0d50-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0d50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0d50-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0d50-113">Not Supported.</span></span>                         |
| <span data-ttu-id="a0d50-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="a0d50-114">Application</span></span>                            | <span data-ttu-id="a0d50-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a0d50-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="a0d50-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0d50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0d50-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0d50-117">Optional query parameters</span></span>
<span data-ttu-id="a0d50-118">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="a0d50-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0d50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0d50-119">Request headers</span></span>
| <span data-ttu-id="a0d50-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a0d50-120">Name</span></span>          | <span data-ttu-id="a0d50-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a0d50-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a0d50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0d50-122">Authorization</span></span> | <span data-ttu-id="a0d50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0d50-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0d50-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0d50-125">Request body</span></span>
<span data-ttu-id="a0d50-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0d50-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0d50-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0d50-127">Response</span></span>
<span data-ttu-id="a0d50-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [call](../resources/call.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0d50-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d50-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a0d50-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0d50-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0d50-130">Request</span></span>
<span data-ttu-id="a0d50-131">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0d50-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="a0d50-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0d50-132">Response</span></span>

> <span data-ttu-id="a0d50-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0d50-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/call-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
