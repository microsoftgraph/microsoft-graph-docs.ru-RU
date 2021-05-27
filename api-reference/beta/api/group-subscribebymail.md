---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 983f0ca44050f60e28bdb642c65f44cadb39b457
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681272"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="69f55-103">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="69f55-103">group: subscribeByMail</span></span>

<span data-ttu-id="69f55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f55-105">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="69f55-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="69f55-106">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="69f55-106">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="69f55-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69f55-107">Permissions</span></span>
<span data-ttu-id="69f55-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69f55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69f55-110">Permission type</span></span>      | <span data-ttu-id="69f55-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69f55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69f55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69f55-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f55-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69f55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69f55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f55-115">Not supported.</span></span>    |
|<span data-ttu-id="69f55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69f55-116">Application</span></span> | <span data-ttu-id="69f55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69f55-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69f55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69f55-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="69f55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69f55-119">Request headers</span></span>
| <span data-ttu-id="69f55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69f55-120">Header</span></span>       | <span data-ttu-id="69f55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69f55-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69f55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69f55-122">Authorization</span></span>  | <span data-ttu-id="69f55-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69f55-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="69f55-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="69f55-125">Prefer</span></span> | <span data-ttu-id="69f55-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="69f55-126">return=minimal.</span></span> <span data-ttu-id="69f55-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69f55-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="69f55-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="69f55-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="69f55-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69f55-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="69f55-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f55-130">Response</span></span>
<span data-ttu-id="69f55-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="69f55-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f55-133">Пример</span><span class="sxs-lookup"><span data-stu-id="69f55-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="69f55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="69f55-134">Request</span></span>
<span data-ttu-id="69f55-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69f55-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69f55-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="69f55-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="69f55-137">C#</span><span class="sxs-lookup"><span data-stu-id="69f55-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69f55-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69f55-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69f55-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69f55-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69f55-140">Java</span><span class="sxs-lookup"><span data-stu-id="69f55-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="69f55-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="69f55-141">Response</span></span>
<span data-ttu-id="69f55-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69f55-142">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


