---
title: Получение участника
description: Получение свойств и связей объекта **участника** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 68d385a70ee359ccdf5307a70f557e75a82a1e37
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523828"
---
# <a name="get-participant"></a><span data-ttu-id="2316b-103">Получение участника</span><span class="sxs-lookup"><span data-stu-id="2316b-103">Get participant</span></span>

<span data-ttu-id="2316b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2316b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2316b-105">Получение свойств и связей объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="2316b-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2316b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2316b-106">Permissions</span></span>

| <span data-ttu-id="2316b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2316b-107">Permission type</span></span> | <span data-ttu-id="2316b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2316b-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="2316b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2316b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="2316b-110">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2316b-110">Not Supported</span></span>        |
| <span data-ttu-id="2316b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2316b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2316b-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2316b-112">Not Supported</span></span>        |
| <span data-ttu-id="2316b-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="2316b-113">Application</span></span>     | <span data-ttu-id="2316b-114">Нет</span><span class="sxs-lookup"><span data-stu-id="2316b-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2316b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2316b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="2316b-116">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2316b-116">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2316b-117">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="2316b-117">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2316b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2316b-118">Optional query parameters</span></span>
<span data-ttu-id="2316b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2316b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2316b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2316b-120">Request headers</span></span>
| <span data-ttu-id="2316b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2316b-121">Name</span></span>          | <span data-ttu-id="2316b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2316b-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2316b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2316b-123">Authorization</span></span> | <span data-ttu-id="2316b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2316b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2316b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2316b-126">Request body</span></span>
<span data-ttu-id="2316b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2316b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2316b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2316b-128">Response</span></span>
<span data-ttu-id="2316b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [участника](../resources/participant.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2316b-129">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2316b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2316b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2316b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2316b-131">Request</span></span>
<span data-ttu-id="2316b-132">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2316b-132">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2316b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2316b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="2316b-134">C#</span><span class="sxs-lookup"><span data-stu-id="2316b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2316b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2316b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2316b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2316b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2316b-137">Java</span><span class="sxs-lookup"><span data-stu-id="2316b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2316b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2316b-138">Response</span></span>

> <span data-ttu-id="2316b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2316b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.type":"#microsoft.graph.participant",
   "info":{
      "@odata.type":"#microsoft.graph.participantInfo",
      "identity":{
         "@odata.type":"#microsoft.graph.identitySet",
         "application":{
            "@odata.type":"#microsoft.graph.identity",
            "displayName":"Display Name",
            "id":"278405a3-f568-4b3e-b684-009193463064",
            "tenantId":"72f988bf-86f1-41af-91ab-2d7cd011db47"
            },
         "user":null,
         "device":null,
         "phone":null
      },
      "id":null,
      "platformId": "4505"
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
   "id":"7e1b4346-85a6-4bdd-abe3-d11c5d420efe",
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/participants/$entity",
   "metadata":null,
   "recordingInfo":null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


