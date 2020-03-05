---
title: 'group: resetUnseenCount'
description: Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения. Поддерживается только для групп Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c6500e7258026578e2adde35d0f194d1c42f9281
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418239"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="db04c-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="db04c-104">group: resetUnseenCount</span></span>

<span data-ttu-id="db04c-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db04c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db04c-106">Сброс свойства unseenCount всех записей, которые пользователь не просматривал со своего предыдущего посещения.</span><span class="sxs-lookup"><span data-stu-id="db04c-106">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="db04c-107">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="db04c-107">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="db04c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db04c-108">Permissions</span></span>
<span data-ttu-id="db04c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db04c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db04c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db04c-111">Permission type</span></span>      | <span data-ttu-id="db04c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db04c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db04c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db04c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db04c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db04c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="db04c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db04c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db04c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db04c-116">Not supported.</span></span>    |
|<span data-ttu-id="db04c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db04c-117">Application</span></span> | <span data-ttu-id="db04c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db04c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db04c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db04c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="db04c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db04c-120">Request headers</span></span>
| <span data-ttu-id="db04c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db04c-121">Header</span></span>       | <span data-ttu-id="db04c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db04c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db04c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db04c-123">Authorization</span></span>  | <span data-ttu-id="db04c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db04c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="db04c-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="db04c-126">Prefer</span></span> | <span data-ttu-id="db04c-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="db04c-127">return=minimal.</span></span> <span data-ttu-id="db04c-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db04c-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="db04c-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="db04c-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="db04c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db04c-130">Request body</span></span>
<span data-ttu-id="db04c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db04c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db04c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="db04c-132">Response</span></span>
<span data-ttu-id="db04c-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db04c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db04c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="db04c-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="db04c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="db04c-136">Request</span></span>
<span data-ttu-id="db04c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db04c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db04c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="db04c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="db04c-139">C#</span><span class="sxs-lookup"><span data-stu-id="db04c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db04c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db04c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db04c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db04c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="db04c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="db04c-142">Response</span></span>
<span data-ttu-id="db04c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db04c-143">The following is an example of the response.</span></span> 
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
