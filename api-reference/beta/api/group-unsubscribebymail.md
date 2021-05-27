---
title: 'group: unsubscribeByMail'
description: Вызов этого метода отключит текущего пользователя для получения уведомлений электронной почты для этой группы о новых сообщениях, событиях и файлах в этой группе.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9a40ba67f5628be6ef25cc4b484b9c84ad71ebb7
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681265"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="44b7d-103">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="44b7d-103">group: unsubscribeByMail</span></span>

<span data-ttu-id="44b7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44b7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44b7d-105">Вызов этого метода отключит текущего пользователя для получения уведомлений электронной почты для этой группы о новых сообщениях, событиях и файлах в этой группе.</span><span class="sxs-lookup"><span data-stu-id="44b7d-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="44b7d-106">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="44b7d-106">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="44b7d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44b7d-107">Permissions</span></span>
<span data-ttu-id="44b7d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44b7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44b7d-110">Permission type</span></span>      | <span data-ttu-id="44b7d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44b7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44b7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44b7d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b7d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44b7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44b7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44b7d-115">Not supported.</span></span>    |
|<span data-ttu-id="44b7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44b7d-116">Application</span></span> | <span data-ttu-id="44b7d-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b7d-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44b7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44b7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="44b7d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44b7d-119">Request headers</span></span>
| <span data-ttu-id="44b7d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44b7d-120">Header</span></span>       | <span data-ttu-id="44b7d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44b7d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44b7d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44b7d-122">Authorization</span></span>  | <span data-ttu-id="44b7d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44b7d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="44b7d-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="44b7d-125">Prefer</span></span> | <span data-ttu-id="44b7d-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="44b7d-126">return=minimal.</span></span> <span data-ttu-id="44b7d-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="44b7d-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="44b7d-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="44b7d-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="44b7d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44b7d-129">Request body</span></span>
 <span data-ttu-id="44b7d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44b7d-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="44b7d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="44b7d-131">Response</span></span>
<span data-ttu-id="44b7d-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="44b7d-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b7d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="44b7d-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="44b7d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="44b7d-135">Request</span></span>
<span data-ttu-id="44b7d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44b7d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44b7d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="44b7d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="44b7d-138">C#</span><span class="sxs-lookup"><span data-stu-id="44b7d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44b7d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44b7d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44b7d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44b7d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44b7d-141">Java</span><span class="sxs-lookup"><span data-stu-id="44b7d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44b7d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="44b7d-142">Response</span></span>
<span data-ttu-id="44b7d-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="44b7d-143">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


