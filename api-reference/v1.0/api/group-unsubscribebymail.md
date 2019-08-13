---
title: 'group: unsubscribeByMail'
description: 'С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a382c8d209835eb295899d2bdd789bf3665f50fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364546"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="73b8f-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="73b8f-104">group: unsubscribeByMail</span></span>
<span data-ttu-id="73b8f-p102">С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="73b8f-p102">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73b8f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73b8f-107">Permissions</span></span>
<span data-ttu-id="73b8f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73b8f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73b8f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73b8f-110">Permission type</span></span>      | <span data-ttu-id="73b8f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73b8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b8f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73b8f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73b8f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b8f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73b8f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73b8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b8f-115">Not supported.</span></span>    |
|<span data-ttu-id="73b8f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73b8f-116">Application</span></span> | <span data-ttu-id="73b8f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b8f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b8f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73b8f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="73b8f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73b8f-119">Request headers</span></span>
| <span data-ttu-id="73b8f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73b8f-120">Header</span></span>       | <span data-ttu-id="73b8f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73b8f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73b8f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73b8f-122">Authorization</span></span>  | <span data-ttu-id="73b8f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73b8f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73b8f-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="73b8f-125">Prefer</span></span> | <span data-ttu-id="73b8f-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="73b8f-126">return=minimal.</span></span> <span data-ttu-id="73b8f-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73b8f-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="73b8f-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="73b8f-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="73b8f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73b8f-129">Request body</span></span>
<span data-ttu-id="73b8f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73b8f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b8f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="73b8f-131">Response</span></span>
<span data-ttu-id="73b8f-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="73b8f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b8f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="73b8f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="73b8f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="73b8f-135">Request</span></span>
<span data-ttu-id="73b8f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73b8f-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73b8f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="73b8f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73b8f-138">C#</span><span class="sxs-lookup"><span data-stu-id="73b8f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73b8f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73b8f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73b8f-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="73b8f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73b8f-141">Java</span><span class="sxs-lookup"><span data-stu-id="73b8f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73b8f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="73b8f-142">Response</span></span>
<span data-ttu-id="73b8f-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73b8f-143">The following is an example of the response.</span></span> 
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
