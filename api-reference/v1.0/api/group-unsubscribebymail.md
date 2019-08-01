---
title: 'group: unsubscribeByMail'
description: 'С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c0eaeb672ae08a7c7a671c214c726cb0f3cba30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014713"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="f3c99-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="f3c99-104">group: unsubscribeByMail</span></span>
<span data-ttu-id="f3c99-p102">С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="f3c99-p102">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f3c99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c99-107">Permissions</span></span>
<span data-ttu-id="f3c99-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3c99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c99-110">Permission type</span></span>      | <span data-ttu-id="f3c99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f3c99-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3c99-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f3c99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3c99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c99-115">Not supported.</span></span>    |
|<span data-ttu-id="f3c99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c99-116">Application</span></span> | <span data-ttu-id="f3c99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c99-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3c99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="f3c99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c99-119">Request headers</span></span>
| <span data-ttu-id="f3c99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c99-120">Header</span></span>       | <span data-ttu-id="f3c99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3c99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c99-122">Authorization</span></span>  | <span data-ttu-id="f3c99-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c99-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f3c99-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="f3c99-125">Prefer</span></span> | <span data-ttu-id="f3c99-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="f3c99-126">return=minimal.</span></span> <span data-ttu-id="f3c99-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3c99-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f3c99-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="f3c99-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f3c99-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3c99-129">Request body</span></span>
<span data-ttu-id="f3c99-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3c99-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3c99-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c99-131">Response</span></span>
<span data-ttu-id="f3c99-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f3c99-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3c99-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c99-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f3c99-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c99-135">Request</span></span>
<span data-ttu-id="f3c99-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c99-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f3c99-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3c99-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3c99-138">C#</span><span class="sxs-lookup"><span data-stu-id="f3c99-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3c99-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3c99-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3c99-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f3c99-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f3c99-141">Java</span><span class="sxs-lookup"><span data-stu-id="f3c99-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f3c99-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c99-142">Response</span></span>
<span data-ttu-id="f3c99-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3c99-143">The following is an example of the response.</span></span> 
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
