---
title: 'group: resetUnseenCount'
description: Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ff1f80d8e716f0fe16ae4e34d40b8f40942f6e32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396310"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="f5cd8-103">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="f5cd8-103">group: resetUnseenCount</span></span>

<span data-ttu-id="f5cd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5cd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5cd8-105">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="f5cd8-106">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-106">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5cd8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5cd8-107">Permissions</span></span>
<span data-ttu-id="f5cd8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5cd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5cd8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5cd8-110">Permission type</span></span>      | <span data-ttu-id="f5cd8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5cd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5cd8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5cd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5cd8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5cd8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5cd8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5cd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5cd8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-115">Not supported.</span></span>    |
|<span data-ttu-id="f5cd8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5cd8-116">Application</span></span> | <span data-ttu-id="f5cd8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5cd8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5cd8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="f5cd8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5cd8-119">Request headers</span></span>
| <span data-ttu-id="f5cd8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5cd8-120">Header</span></span>       | <span data-ttu-id="f5cd8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f5cd8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5cd8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5cd8-122">Authorization</span></span>  | <span data-ttu-id="f5cd8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5cd8-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="f5cd8-125">Prefer</span></span> | <span data-ttu-id="f5cd8-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-126">return=minimal.</span></span> <span data-ttu-id="f5cd8-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f5cd8-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f5cd8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5cd8-129">Request body</span></span>
<span data-ttu-id="f5cd8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5cd8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5cd8-131">Response</span></span>
<span data-ttu-id="f5cd8-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5cd8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f5cd8-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5cd8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5cd8-135">Request</span></span>
<span data-ttu-id="f5cd8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5cd8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5cd8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="f5cd8-138">C#</span><span class="sxs-lookup"><span data-stu-id="f5cd8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5cd8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5cd8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5cd8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5cd8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f5cd8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5cd8-141">Response</span></span>
<span data-ttu-id="f5cd8-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5cd8-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
