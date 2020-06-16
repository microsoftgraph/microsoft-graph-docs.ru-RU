---
title: Список цепочек
description: Получение всех цепочек в групповой беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b71fb32f786ddfe0736ef6e14dc44d8c0e2d12f0
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44743909"
---
# <a name="list-threads"></a><span data-ttu-id="08f82-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="08f82-103">List threads</span></span>

<span data-ttu-id="08f82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08f82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f82-105">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="08f82-105">Get all the threads in a group conversation.</span></span>
<span data-ttu-id="08f82-106">Примечание. Вы также можете [получить все цепочки группы](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="08f82-106">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="08f82-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08f82-107">Permissions</span></span>
<span data-ttu-id="08f82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08f82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08f82-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08f82-110">Permission type</span></span>      | <span data-ttu-id="08f82-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08f82-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08f82-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08f82-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08f82-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f82-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08f82-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08f82-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08f82-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08f82-115">Not supported.</span></span>    |
|<span data-ttu-id="08f82-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08f82-116">Application</span></span> | <span data-ttu-id="08f82-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f82-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08f82-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08f82-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08f82-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08f82-119">Optional query parameters</span></span>
<span data-ttu-id="08f82-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08f82-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08f82-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08f82-121">Request headers</span></span>
| <span data-ttu-id="08f82-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08f82-122">Header</span></span>       | <span data-ttu-id="08f82-123">Значение</span><span class="sxs-lookup"><span data-stu-id="08f82-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08f82-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08f82-124">Authorization</span></span>  | <span data-ttu-id="08f82-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08f82-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08f82-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08f82-127">Request body</span></span>
<span data-ttu-id="08f82-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08f82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08f82-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="08f82-129">Response</span></span>

<span data-ttu-id="08f82-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08f82-130">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08f82-131">Пример</span><span class="sxs-lookup"><span data-stu-id="08f82-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08f82-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="08f82-132">Request</span></span>
<span data-ttu-id="08f82-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08f82-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08f82-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="08f82-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="08f82-135">C#</span><span class="sxs-lookup"><span data-stu-id="08f82-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08f82-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08f82-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08f82-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08f82-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="08f82-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="08f82-138">Response</span></span>
<span data-ttu-id="08f82-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08f82-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
