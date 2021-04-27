---
title: Список rejectedSenders
description: 'Получение списка пользователей или групп, включенных в список запрещенных отправителей для этой группы. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 657f6a847d8d00b8543a2d560e5a6eac955243c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041458"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="8495d-103">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="8495d-103">List rejectedSenders</span></span>

<span data-ttu-id="8495d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8495d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8495d-105">Получение списка пользователей или групп, включенных в список запрещенных отправителей для этой группы.</span><span class="sxs-lookup"><span data-stu-id="8495d-105">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="8495d-p101">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="8495d-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8495d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8495d-108">Permissions</span></span>
<span data-ttu-id="8495d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8495d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8495d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8495d-111">Permission type</span></span>      | <span data-ttu-id="8495d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8495d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8495d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8495d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8495d-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8495d-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8495d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8495d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8495d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8495d-116">Not supported.</span></span>    |
|<span data-ttu-id="8495d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8495d-117">Application</span></span> | <span data-ttu-id="8495d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8495d-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8495d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8495d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8495d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8495d-120">Optional query parameters</span></span>
<span data-ttu-id="8495d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8495d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8495d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8495d-122">Request headers</span></span>
| <span data-ttu-id="8495d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8495d-123">Header</span></span>       | <span data-ttu-id="8495d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8495d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8495d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8495d-125">Authorization</span></span>  | <span data-ttu-id="8495d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8495d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8495d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8495d-128">Request body</span></span>
<span data-ttu-id="8495d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8495d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8495d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8495d-130">Response</span></span>
<span data-ttu-id="8495d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8495d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8495d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8495d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8495d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8495d-133">Request</span></span>
<span data-ttu-id="8495d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8495d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8495d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8495d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```
# <a name="c"></a>[<span data-ttu-id="8495d-136">C#</span><span class="sxs-lookup"><span data-stu-id="8495d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8495d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8495d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8495d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8495d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8495d-139">Java</span><span class="sxs-lookup"><span data-stu-id="8495d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8495d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8495d-140">Response</span></span>
<span data-ttu-id="8495d-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8495d-141">The following is an example of the response.</span></span>
><span data-ttu-id="8495d-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8495d-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


