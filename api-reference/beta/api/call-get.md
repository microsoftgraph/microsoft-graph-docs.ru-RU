---
title: Начало звонка
description: Извлечение свойств и связи объекта вызова.
author: VinodRavichandran
ms.openlocfilehash: df97b69f87a1562e56a96d84de1af740ab0aff65
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380326"
---
# <a name="get-call"></a><span data-ttu-id="2e348-103">Начало звонка</span><span class="sxs-lookup"><span data-stu-id="2e348-103">Get call</span></span>

> <span data-ttu-id="2e348-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2e348-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e348-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e348-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e348-106">Извлечение свойств и связи объекта вызова.</span><span class="sxs-lookup"><span data-stu-id="2e348-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e348-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e348-107">Permissions</span></span>
<span data-ttu-id="2e348-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e348-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e348-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e348-110">Permission type</span></span> | <span data-ttu-id="2e348-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e348-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2e348-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e348-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e348-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e348-113">Not Supported.</span></span>                         |
| <span data-ttu-id="2e348-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e348-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e348-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e348-115">Not Supported.</span></span>                         |
| <span data-ttu-id="2e348-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e348-116">Application</span></span>                            | <span data-ttu-id="2e348-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2e348-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="2e348-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e348-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e348-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e348-119">Optional query parameters</span></span>
<span data-ttu-id="2e348-120">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="2e348-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e348-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e348-121">Request headers</span></span>
| <span data-ttu-id="2e348-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2e348-122">Name</span></span>          | <span data-ttu-id="2e348-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2e348-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2e348-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e348-124">Authorization</span></span> | <span data-ttu-id="2e348-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e348-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e348-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e348-127">Request body</span></span>
<span data-ttu-id="2e348-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e348-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e348-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e348-129">Response</span></span>
<span data-ttu-id="2e348-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [call](../resources/call.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e348-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e348-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e348-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e348-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e348-132">Request</span></span>
<span data-ttu-id="2e348-133">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e348-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="2e348-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e348-134">Response</span></span>

> <span data-ttu-id="2e348-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e348-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
