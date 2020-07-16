---
title: 'group: addFavorite'
description: Добавление группы в список избранных групп текущего пользователя. Поддерживается только для групп Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7879b5dc724f784addecb93cab137935143a4dd6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895890"
---
# <a name="group-addfavorite"></a><span data-ttu-id="bb1fe-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="bb1fe-104">group: addFavorite</span></span>

<span data-ttu-id="bb1fe-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb1fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb1fe-106">Добавление группы в список избранных групп текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-106">Add the group to the list of the current user's favorite groups.</span></span> <span data-ttu-id="bb1fe-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb1fe-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb1fe-108">Permissions</span></span>
<span data-ttu-id="bb1fe-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb1fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb1fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb1fe-111">Permission type</span></span>      | <span data-ttu-id="bb1fe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb1fe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb1fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb1fe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb1fe-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb1fe-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb1fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb1fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb1fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-116">Not supported.</span></span>    |
|<span data-ttu-id="bb1fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb1fe-117">Application</span></span> | <span data-ttu-id="bb1fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb1fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb1fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="bb1fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb1fe-120">Request headers</span></span>
| <span data-ttu-id="bb1fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb1fe-121">Header</span></span>       | <span data-ttu-id="bb1fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb1fe-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb1fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb1fe-123">Authorization</span></span>  | <span data-ttu-id="bb1fe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bb1fe-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="bb1fe-126">Prefer</span></span> | <span data-ttu-id="bb1fe-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-127">return=minimal.</span></span> <span data-ttu-id="bb1fe-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="bb1fe-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="bb1fe-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb1fe-130">Request body</span></span>
<span data-ttu-id="bb1fe-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb1fe-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb1fe-132">Response</span></span>
<span data-ttu-id="bb1fe-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb1fe-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bb1fe-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb1fe-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb1fe-136">Request</span></span>
<span data-ttu-id="bb1fe-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb1fe-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb1fe-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```
# <a name="c"></a>[<span data-ttu-id="bb1fe-139">C#</span><span class="sxs-lookup"><span data-stu-id="bb1fe-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-addfavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb1fe-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb1fe-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-addfavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb1fe-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb1fe-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-addfavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb1fe-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb1fe-142">Response</span></span>
<span data-ttu-id="bb1fe-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bb1fe-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
