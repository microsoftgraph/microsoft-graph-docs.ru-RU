---
title: Список участников
description: Получение списка объектов участников в вызове.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 26ff72167cf783eb96ab4c7ec258172581134172
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871435"
---
# <a name="list-participants"></a><span data-ttu-id="0fa68-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="0fa68-103">List participants</span></span>

<span data-ttu-id="0fa68-104">Получение списка объектов участников в вызове.</span><span class="sxs-lookup"><span data-stu-id="0fa68-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa68-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0fa68-105">Permissions</span></span>

| <span data-ttu-id="0fa68-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fa68-106">Permission type</span></span> | <span data-ttu-id="0fa68-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fa68-107">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="0fa68-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fa68-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fa68-109">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0fa68-109">Not Supported</span></span>        |
| <span data-ttu-id="0fa68-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fa68-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa68-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0fa68-111">Not Supported</span></span>        |
| <span data-ttu-id="0fa68-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="0fa68-112">Application</span></span>     | <span data-ttu-id="0fa68-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="0fa68-113">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="0fa68-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fa68-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fa68-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0fa68-115">Optional query parameters</span></span>

<span data-ttu-id="0fa68-116">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa68-116">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fa68-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fa68-117">Request headers</span></span>

| <span data-ttu-id="0fa68-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0fa68-118">Name</span></span>          | <span data-ttu-id="0fa68-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0fa68-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="0fa68-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fa68-120">Authorization</span></span> | <span data-ttu-id="0fa68-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fa68-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fa68-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fa68-123">Request body</span></span>

<span data-ttu-id="0fa68-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fa68-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fa68-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fa68-125">Response</span></span>

<span data-ttu-id="0fa68-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов- [участников](../resources/participant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fa68-126">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa68-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0fa68-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa68-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fa68-128">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fa68-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa68-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fa68-130">C#</span><span class="sxs-lookup"><span data-stu-id="0fa68-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fa68-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa68-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fa68-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa68-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fa68-133">Java</span><span class="sxs-lookup"><span data-stu-id="0fa68-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="0fa68-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fa68-134">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "id":"f2fa86af-3c51-4bc2-8fc0-475452d9764f",
                  "displayName":null
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"eec3812a-fdc3-4fb4-825c-a06c9f35414e"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"3",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"a7ebfb2d-871e-419c-87af-27290b22e8db",
         "metadata":null
      },
      {
         "@odata.type":"#microsoft.graph.participant",
         "info":{
            "@odata.type":"#microsoft.graph.participantInfo",
            "identity":{
               "@odata.type":"#microsoft.graph.identitySet",
               "application":{
                  "@odata.type":"#microsoft.graph.identity",
                  "displayName":"Test Participant",
                  "id":"ef43e42b-4c05-4594-9756-1edb3ccbc989"
               },
               "user":null,
               "device":null,
               "phone":null
            },
            "id":"278405a3-f568-4b3e-b684-009193463064"
         },
         "mediaStreams":[
            {
               "@odata.type":"#microsoft.graph.mediaStream",
               "mediaType":"audio",
               "sourceId":"1",
               "direction":"sendReceive",
               "serverMuted":false,
               "label":null
            }
         ],
         "isMuted":false,
         "isInLobby":false,
         "id":"1e126418-44a0-4a94-a6f8-0efe1ad71acb",
         "metadata":null
      }
   ],
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
