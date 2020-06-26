---
title: 'group: unsubscribeByMail'
description: 'С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Microsoft 365. '
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: afbee22fc9c51cd9b7428b89677907efc3786c1c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897122"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="f68a0-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="f68a0-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="f68a0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f68a0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f68a0-106">С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="f68a0-106">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="f68a0-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f68a0-107">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f68a0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f68a0-108">Permissions</span></span>
<span data-ttu-id="f68a0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f68a0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f68a0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f68a0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f68a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f68a0-111">Permission type</span></span>      | <span data-ttu-id="f68a0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f68a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f68a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f68a0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f68a0-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f68a0-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f68a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f68a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f68a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f68a0-116">Not supported.</span></span>    |
|<span data-ttu-id="f68a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f68a0-117">Application</span></span> | <span data-ttu-id="f68a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f68a0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f68a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f68a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="f68a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f68a0-120">Request headers</span></span>
| <span data-ttu-id="f68a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f68a0-121">Header</span></span>       | <span data-ttu-id="f68a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f68a0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f68a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f68a0-123">Authorization</span></span>  | <span data-ttu-id="f68a0-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f68a0-124">Bearer {token}.</span></span> <span data-ttu-id="f68a0-125">Required.</span><span class="sxs-lookup"><span data-stu-id="f68a0-125">Required.</span></span>  |
| <span data-ttu-id="f68a0-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="f68a0-126">Prefer</span></span> | <span data-ttu-id="f68a0-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="f68a0-127">return=minimal.</span></span> <span data-ttu-id="f68a0-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f68a0-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f68a0-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f68a0-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f68a0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f68a0-130">Request body</span></span>
<span data-ttu-id="f68a0-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f68a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f68a0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f68a0-132">Response</span></span>
<span data-ttu-id="f68a0-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="f68a0-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="f68a0-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="f68a0-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f68a0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f68a0-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f68a0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f68a0-136">Request</span></span>
<span data-ttu-id="f68a0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f68a0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f68a0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f68a0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="f68a0-139">C#</span><span class="sxs-lookup"><span data-stu-id="f68a0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f68a0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f68a0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f68a0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f68a0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f68a0-142">Java</span><span class="sxs-lookup"><span data-stu-id="f68a0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f68a0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f68a0-143">Response</span></span>
<span data-ttu-id="f68a0-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f68a0-144">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
