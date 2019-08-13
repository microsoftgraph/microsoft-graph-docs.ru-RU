---
title: 'group: removeFavorite'
description: Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 941edb23d6c029e6b1b81fcfa56704ceb9d53388
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323180"
---
# <a name="group-removefavorite"></a><span data-ttu-id="08467-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="08467-104">group: removeFavorite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08467-p102">Удаление группы из списка избранных групп текущего пользователя. Поддерживается только для Групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="08467-p102">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="08467-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08467-107">Permissions</span></span>
<span data-ttu-id="08467-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08467-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08467-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08467-110">Permission type</span></span>      | <span data-ttu-id="08467-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08467-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08467-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08467-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08467-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08467-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="08467-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08467-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08467-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08467-115">Not supported.</span></span>    |
|<span data-ttu-id="08467-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08467-116">Application</span></span> | <span data-ttu-id="08467-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08467-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08467-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08467-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="08467-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08467-119">Request headers</span></span>
| <span data-ttu-id="08467-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08467-120">Header</span></span>       | <span data-ttu-id="08467-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08467-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08467-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08467-122">Authorization</span></span>  | <span data-ttu-id="08467-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08467-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08467-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="08467-125">Prefer</span></span> | <span data-ttu-id="08467-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="08467-126">return=minimal.</span></span> <span data-ttu-id="08467-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="08467-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="08467-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="08467-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="08467-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="08467-129">Request body</span></span>
<span data-ttu-id="08467-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08467-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08467-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="08467-131">Response</span></span>
<span data-ttu-id="08467-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08467-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08467-134">Пример</span><span class="sxs-lookup"><span data-stu-id="08467-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="08467-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="08467-135">Request</span></span>
<span data-ttu-id="08467-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08467-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08467-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="08467-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08467-138">C#</span><span class="sxs-lookup"><span data-stu-id="08467-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08467-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08467-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08467-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="08467-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08467-141">Java</span><span class="sxs-lookup"><span data-stu-id="08467-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="08467-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="08467-142">Response</span></span>
<span data-ttu-id="08467-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08467-143">The following is an example of the response.</span></span>
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
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
