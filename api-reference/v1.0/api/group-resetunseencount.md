---
title: 'group: resetUnseenCount'
description: Сброс unseenCount всех записей, которые текущий пользователь не просматривал со времени своего предыдущего посещения. Поддерживается только для групп Office 365.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 66c0f6009e5f25529d2dcb787457a45df8281d1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516944"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="278fd-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="278fd-104">group: resetUnseenCount</span></span>

<span data-ttu-id="278fd-105">Пространство имен: Microsoft. Graph сброс значений unseencount всех сообщений, которые текущий пользователь не видел с момента последнего посещения.</span><span class="sxs-lookup"><span data-stu-id="278fd-105">Namespace: microsoft.graph Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="278fd-106">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="278fd-106">Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="278fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="278fd-107">Permissions</span></span>
<span data-ttu-id="278fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="278fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="278fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="278fd-110">Permission type</span></span>      | <span data-ttu-id="278fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="278fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="278fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="278fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="278fd-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="278fd-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="278fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="278fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="278fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="278fd-115">Not supported.</span></span>    |
|<span data-ttu-id="278fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="278fd-116">Application</span></span> | <span data-ttu-id="278fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="278fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="278fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="278fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="278fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="278fd-119">Request headers</span></span>
| <span data-ttu-id="278fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="278fd-120">Header</span></span>       | <span data-ttu-id="278fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="278fd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="278fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="278fd-122">Authorization</span></span>  | <span data-ttu-id="278fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="278fd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="278fd-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="278fd-125">Prefer</span></span> | <span data-ttu-id="278fd-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="278fd-126">return=minimal.</span></span> <span data-ttu-id="278fd-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="278fd-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="278fd-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="278fd-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="278fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="278fd-129">Request body</span></span>
<span data-ttu-id="278fd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="278fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="278fd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="278fd-131">Response</span></span>
<span data-ttu-id="278fd-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="278fd-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="278fd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="278fd-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="278fd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="278fd-135">Request</span></span>
<span data-ttu-id="278fd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="278fd-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="278fd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="278fd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="278fd-138">C#</span><span class="sxs-lookup"><span data-stu-id="278fd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="278fd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="278fd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="278fd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="278fd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="278fd-141">Java</span><span class="sxs-lookup"><span data-stu-id="278fd-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="278fd-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="278fd-142">Response</span></span>
<span data-ttu-id="278fd-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="278fd-143">The following is an example of the response.</span></span> 
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
