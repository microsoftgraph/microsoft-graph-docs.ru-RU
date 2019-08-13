---
title: Получение цепочки беседы
description: Получение объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2de55721c5029cbab0ba396a6fc99e682bfc0953
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337393"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="a8562-103">Получение цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="a8562-103">Get conversation thread</span></span>
<span data-ttu-id="a8562-104">Получение объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="a8562-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8562-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8562-105">Permissions</span></span>
<span data-ttu-id="a8562-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8562-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8562-108">Permission type</span></span>      | <span data-ttu-id="a8562-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8562-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8562-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8562-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8562-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8562-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8562-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8562-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8562-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8562-113">Not supported.</span></span>    |
|<span data-ttu-id="a8562-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8562-114">Application</span></span> | <span data-ttu-id="a8562-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8562-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8562-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8562-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8562-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8562-117">Optional query parameters</span></span>
<span data-ttu-id="a8562-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8562-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8562-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8562-119">Request headers</span></span>
| <span data-ttu-id="a8562-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8562-120">Header</span></span>       | <span data-ttu-id="a8562-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a8562-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8562-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8562-122">Authorization</span></span>  | <span data-ttu-id="a8562-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8562-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8562-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8562-125">Request body</span></span>
<span data-ttu-id="a8562-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8562-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8562-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8562-127">Response</span></span>
<span data-ttu-id="a8562-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [thread](../resources/conversationthread.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8562-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8562-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a8562-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a8562-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8562-130">Request</span></span>
<span data-ttu-id="a8562-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8562-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8562-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8562-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8562-133">C#</span><span class="sxs-lookup"><span data-stu-id="a8562-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8562-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8562-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8562-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a8562-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8562-136">Java</span><span class="sxs-lookup"><span data-stu-id="a8562-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8562-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8562-137">Response</span></span>
<span data-ttu-id="a8562-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8562-138">The following is an example of the response.</span></span>
><span data-ttu-id="a8562-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8562-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
