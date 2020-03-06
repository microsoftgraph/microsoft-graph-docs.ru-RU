---
title: Список участников
description: Получение списка объектов участников в вызове.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e26603bba1b8f441de53eaf6ecc45b2d579542d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518709"
---
# <a name="list-participants"></a><span data-ttu-id="ca7cf-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="ca7cf-103">List participants</span></span>

<span data-ttu-id="ca7cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca7cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca7cf-105">Получение списка объектов участников в вызове.</span><span class="sxs-lookup"><span data-stu-id="ca7cf-105">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca7cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca7cf-106">Permissions</span></span>

| <span data-ttu-id="ca7cf-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca7cf-107">Permission type</span></span> | <span data-ttu-id="ca7cf-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca7cf-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="ca7cf-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca7cf-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca7cf-110">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ca7cf-110">Not Supported</span></span>        |
| <span data-ttu-id="ca7cf-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca7cf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca7cf-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ca7cf-112">Not Supported</span></span>        |
| <span data-ttu-id="ca7cf-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca7cf-113">Application</span></span>     | <span data-ttu-id="ca7cf-114">Нет</span><span class="sxs-lookup"><span data-stu-id="ca7cf-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="ca7cf-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca7cf-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca7cf-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca7cf-116">Optional query parameters</span></span>

<span data-ttu-id="ca7cf-117">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ca7cf-117">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca7cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca7cf-118">Request headers</span></span>

| <span data-ttu-id="ca7cf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ca7cf-119">Name</span></span>          | <span data-ttu-id="ca7cf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ca7cf-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ca7cf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca7cf-121">Authorization</span></span> | <span data-ttu-id="ca7cf-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca7cf-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca7cf-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca7cf-124">Request body</span></span>

<span data-ttu-id="ca7cf-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca7cf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca7cf-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca7cf-126">Response</span></span>

<span data-ttu-id="ca7cf-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов- [участников](../resources/participant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca7cf-127">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca7cf-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ca7cf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca7cf-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca7cf-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca7cf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca7cf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants
```
# <a name="c"></a>[<span data-ttu-id="ca7cf-131">C#</span><span class="sxs-lookup"><span data-stu-id="ca7cf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca7cf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca7cf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca7cf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca7cf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca7cf-134">Java</span><span class="sxs-lookup"><span data-stu-id="ca7cf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="ca7cf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca7cf-135">Response</span></span>

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
