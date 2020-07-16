---
title: 'group: resetUnseenCount'
description: Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения. Поддерживается только для групп Microsoft 365.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3858d98b6ae932043f3ba478f06be9d0e419dd4f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897136"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="d15eb-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="d15eb-104">group: resetUnseenCount</span></span>

<span data-ttu-id="d15eb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15eb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d15eb-106">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения.</span><span class="sxs-lookup"><span data-stu-id="d15eb-106">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="d15eb-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d15eb-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="d15eb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d15eb-108">Permissions</span></span>
<span data-ttu-id="d15eb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d15eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d15eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d15eb-111">Permission type</span></span>      | <span data-ttu-id="d15eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d15eb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d15eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d15eb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d15eb-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15eb-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d15eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d15eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d15eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15eb-116">Not supported.</span></span>    |
|<span data-ttu-id="d15eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d15eb-117">Application</span></span> | <span data-ttu-id="d15eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d15eb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d15eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d15eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="d15eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d15eb-120">Request headers</span></span>
| <span data-ttu-id="d15eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d15eb-121">Header</span></span>       | <span data-ttu-id="d15eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d15eb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d15eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d15eb-123">Authorization</span></span>  | <span data-ttu-id="d15eb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d15eb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d15eb-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="d15eb-126">Prefer</span></span> | <span data-ttu-id="d15eb-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="d15eb-127">return=minimal.</span></span> <span data-ttu-id="d15eb-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d15eb-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="d15eb-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d15eb-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="d15eb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d15eb-130">Request body</span></span>
<span data-ttu-id="d15eb-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d15eb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d15eb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d15eb-132">Response</span></span>
<span data-ttu-id="d15eb-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d15eb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d15eb-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d15eb-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d15eb-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d15eb-136">Request</span></span>
<span data-ttu-id="d15eb-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d15eb-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d15eb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d15eb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="d15eb-139">C#</span><span class="sxs-lookup"><span data-stu-id="d15eb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d15eb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d15eb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d15eb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d15eb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d15eb-142">Java</span><span class="sxs-lookup"><span data-stu-id="d15eb-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d15eb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d15eb-143">Response</span></span>
<span data-ttu-id="d15eb-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d15eb-144">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
