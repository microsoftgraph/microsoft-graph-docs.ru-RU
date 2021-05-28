---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Microsoft 365.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6962dfc37ac546f82f7d4ea99a5c8d0157a981c7
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679885"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="8e91c-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="8e91c-104">group: subscribeByMail</span></span>

<span data-ttu-id="8e91c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e91c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e91c-106">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="8e91c-106">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="8e91c-107">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8e91c-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e91c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e91c-108">Permissions</span></span>
<span data-ttu-id="8e91c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e91c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e91c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e91c-111">Permission type</span></span>      | <span data-ttu-id="8e91c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e91c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e91c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e91c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e91c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e91c-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e91c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e91c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e91c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e91c-116">Not supported.</span></span>    |
|<span data-ttu-id="8e91c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e91c-117">Application</span></span> | <span data-ttu-id="8e91c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e91c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e91c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e91c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="8e91c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e91c-120">Request headers</span></span>
| <span data-ttu-id="8e91c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e91c-121">Header</span></span>       | <span data-ttu-id="8e91c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e91c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e91c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e91c-123">Authorization</span></span>  | <span data-ttu-id="8e91c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e91c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e91c-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="8e91c-126">Prefer</span></span> | <span data-ttu-id="8e91c-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="8e91c-127">return=minimal.</span></span> <span data-ttu-id="8e91c-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e91c-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="8e91c-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8e91c-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="8e91c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e91c-130">Request body</span></span>
<span data-ttu-id="8e91c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e91c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e91c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e91c-132">Response</span></span>
<span data-ttu-id="8e91c-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8e91c-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e91c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8e91c-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8e91c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e91c-136">Request</span></span>
<span data-ttu-id="8e91c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e91c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e91c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e91c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="8e91c-139">C#</span><span class="sxs-lookup"><span data-stu-id="8e91c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e91c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e91c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e91c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e91c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e91c-142">Java</span><span class="sxs-lookup"><span data-stu-id="8e91c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e91c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e91c-143">Response</span></span>
<span data-ttu-id="8e91c-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e91c-144">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

