---
title: Получение цепочки беседы
description: Получение объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 09339f70e42c14dade2648bb5ed2aee1f2b88442
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440563"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="fcb50-103">Получение цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="fcb50-103">Get conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcb50-104">Получение объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="fcb50-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcb50-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcb50-105">Permissions</span></span>
<span data-ttu-id="fcb50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcb50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcb50-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcb50-108">Permission type</span></span>      | <span data-ttu-id="fcb50-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcb50-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcb50-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcb50-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fcb50-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb50-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fcb50-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcb50-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcb50-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcb50-113">Not supported.</span></span>    |
|<span data-ttu-id="fcb50-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcb50-114">Application</span></span> | <span data-ttu-id="fcb50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcb50-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcb50-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcb50-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcb50-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcb50-117">Optional query parameters</span></span>
<span data-ttu-id="fcb50-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcb50-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcb50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcb50-119">Request headers</span></span>
| <span data-ttu-id="fcb50-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcb50-120">Header</span></span>       | <span data-ttu-id="fcb50-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fcb50-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fcb50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcb50-122">Authorization</span></span>  | <span data-ttu-id="fcb50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcb50-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fcb50-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcb50-125">Request body</span></span>
<span data-ttu-id="fcb50-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcb50-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcb50-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcb50-127">Response</span></span>
<span data-ttu-id="fcb50-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [thread](../resources/conversationthread.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcb50-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcb50-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fcb50-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fcb50-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcb50-130">Request</span></span>
<span data-ttu-id="fcb50-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcb50-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fcb50-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcb50-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fcb50-133">C#</span><span class="sxs-lookup"><span data-stu-id="fcb50-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fcb50-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fcb50-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fcb50-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fcb50-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fcb50-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcb50-136">Response</span></span>
<span data-ttu-id="fcb50-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcb50-137">The following is an example of the response.</span></span>
><span data-ttu-id="fcb50-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcb50-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
