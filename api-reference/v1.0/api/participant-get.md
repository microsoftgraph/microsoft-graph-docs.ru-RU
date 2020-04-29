---
title: Получение участника
description: Получение свойств и связей объекта **участника** .
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f5f514f053e73aef0d13c9eb6f3b835e3219a6ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511077"
---
# <a name="get-participant"></a><span data-ttu-id="3363f-103">Получение участника</span><span class="sxs-lookup"><span data-stu-id="3363f-103">Get participant</span></span>

<span data-ttu-id="3363f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3363f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3363f-105">Получение свойств и связей объекта **участника** .</span><span class="sxs-lookup"><span data-stu-id="3363f-105">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3363f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3363f-106">Permissions</span></span>

| <span data-ttu-id="3363f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3363f-107">Permission type</span></span> | <span data-ttu-id="3363f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3363f-108">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="3363f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3363f-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="3363f-110">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3363f-110">Not Supported</span></span>        |
| <span data-ttu-id="3363f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3363f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3363f-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3363f-112">Not Supported</span></span>        |
| <span data-ttu-id="3363f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3363f-113">Application</span></span>     | <span data-ttu-id="3363f-114">Нет</span><span class="sxs-lookup"><span data-stu-id="3363f-114">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="3363f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3363f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3363f-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3363f-116">Optional query parameters</span></span>
<span data-ttu-id="3363f-117">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3363f-117">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3363f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3363f-118">Request headers</span></span>
| <span data-ttu-id="3363f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3363f-119">Name</span></span>          | <span data-ttu-id="3363f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3363f-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3363f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3363f-121">Authorization</span></span> | <span data-ttu-id="3363f-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3363f-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3363f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3363f-124">Request body</span></span>
<span data-ttu-id="3363f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3363f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3363f-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="3363f-126">Response</span></span>
<span data-ttu-id="3363f-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [участника](../resources/participant.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3363f-127">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3363f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3363f-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3363f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3363f-129">Request</span></span>
<span data-ttu-id="3363f-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3363f-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3363f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3363f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants/7e1b4346-85a6-4bdd-abe3-d11c5d420efe
```
# <a name="c"></a>[<span data-ttu-id="3363f-132">C#</span><span class="sxs-lookup"><span data-stu-id="3363f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3363f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3363f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3363f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3363f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3363f-135">Java</span><span class="sxs-lookup"><span data-stu-id="3363f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3363f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3363f-136">Response</span></span>

> <span data-ttu-id="3363f-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3363f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "id":"278405a3-f568-4b3e-b684-009193463064"
            },
         "user":null,
         "device":null,
         "phone":null
      },
      "id":null
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
   "metadata":null
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
