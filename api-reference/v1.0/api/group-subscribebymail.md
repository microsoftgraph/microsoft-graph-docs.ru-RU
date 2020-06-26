---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e3cb0d0a79da9ec246f0da50f17c3987695bb27
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897129"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="63c29-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="63c29-104">group: subscribeByMail</span></span>

<span data-ttu-id="63c29-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63c29-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63c29-106">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="63c29-106">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="63c29-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="63c29-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="63c29-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63c29-108">Permissions</span></span>
<span data-ttu-id="63c29-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="63c29-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="63c29-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63c29-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63c29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63c29-111">Permission type</span></span>      | <span data-ttu-id="63c29-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63c29-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63c29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63c29-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63c29-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63c29-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63c29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63c29-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63c29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c29-116">Not supported.</span></span>    |
|<span data-ttu-id="63c29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63c29-117">Application</span></span> | <span data-ttu-id="63c29-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c29-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63c29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63c29-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="63c29-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63c29-120">Request headers</span></span>
| <span data-ttu-id="63c29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63c29-121">Header</span></span>       | <span data-ttu-id="63c29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63c29-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63c29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63c29-123">Authorization</span></span>  | <span data-ttu-id="63c29-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="63c29-124">Bearer {token}.</span></span> <span data-ttu-id="63c29-125">Required.</span><span class="sxs-lookup"><span data-stu-id="63c29-125">Required.</span></span>  |
| <span data-ttu-id="63c29-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="63c29-126">Prefer</span></span> | <span data-ttu-id="63c29-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="63c29-127">return=minimal.</span></span> <span data-ttu-id="63c29-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="63c29-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="63c29-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="63c29-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="63c29-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63c29-130">Request body</span></span>
<span data-ttu-id="63c29-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63c29-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63c29-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c29-132">Response</span></span>
<span data-ttu-id="63c29-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="63c29-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="63c29-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="63c29-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63c29-135">Пример</span><span class="sxs-lookup"><span data-stu-id="63c29-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="63c29-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="63c29-136">Request</span></span>
<span data-ttu-id="63c29-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63c29-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63c29-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="63c29-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="63c29-139">C#</span><span class="sxs-lookup"><span data-stu-id="63c29-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63c29-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63c29-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63c29-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63c29-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63c29-142">Java</span><span class="sxs-lookup"><span data-stu-id="63c29-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63c29-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c29-143">Response</span></span>
<span data-ttu-id="63c29-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63c29-144">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
