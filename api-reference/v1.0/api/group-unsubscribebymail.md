---
title: 'group: unsubscribeByMail'
description: 'С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365. '
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0c2aece1632ed2ebd59def7e8bd00e56ec5676c0
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168551"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="de575-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="de575-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="de575-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de575-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de575-p102">С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="de575-p102">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="de575-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de575-108">Permissions</span></span>
<span data-ttu-id="de575-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de575-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de575-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de575-111">Permission type</span></span>      | <span data-ttu-id="de575-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de575-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de575-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de575-113">Delegated (work or school account)</span></span> | <span data-ttu-id="de575-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de575-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="de575-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de575-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de575-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de575-116">Not supported.</span></span>    |
|<span data-ttu-id="de575-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de575-117">Application</span></span> | <span data-ttu-id="de575-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de575-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de575-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de575-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="de575-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de575-120">Request headers</span></span>
| <span data-ttu-id="de575-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de575-121">Header</span></span>       | <span data-ttu-id="de575-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de575-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de575-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de575-123">Authorization</span></span>  | <span data-ttu-id="de575-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de575-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de575-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="de575-126">Prefer</span></span> | <span data-ttu-id="de575-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="de575-127">return=minimal.</span></span> <span data-ttu-id="de575-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de575-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="de575-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="de575-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="de575-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de575-130">Request body</span></span>
<span data-ttu-id="de575-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de575-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de575-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="de575-132">Response</span></span>
<span data-ttu-id="de575-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="de575-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de575-135">Пример</span><span class="sxs-lookup"><span data-stu-id="de575-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="de575-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="de575-136">Request</span></span>
<span data-ttu-id="de575-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de575-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de575-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="de575-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="de575-139">C#</span><span class="sxs-lookup"><span data-stu-id="de575-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de575-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de575-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de575-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de575-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de575-142">Java</span><span class="sxs-lookup"><span data-stu-id="de575-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de575-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="de575-143">Response</span></span>
<span data-ttu-id="de575-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="de575-144">The following is an example of the response.</span></span> 
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
