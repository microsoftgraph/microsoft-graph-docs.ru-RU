---
title: 'group: unsubscribeByMail'
description: Вызов этого метода отключит текущего пользователя на получение уведомлений по электронной почте для этой группы о новых публикациях, событиях и файлах в этой группе.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c33a5009a329deb42021fff5a26c4efa445ba26c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895785"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="e149b-103">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="e149b-103">group: unsubscribeByMail</span></span>

<span data-ttu-id="e149b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e149b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e149b-105">Вызов этого метода отключит текущего пользователя на получение уведомлений по электронной почте для этой группы о новых публикациях, событиях и файлах в этой группе.</span><span class="sxs-lookup"><span data-stu-id="e149b-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="e149b-106">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e149b-106">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e149b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e149b-107">Permissions</span></span>
<span data-ttu-id="e149b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e149b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e149b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e149b-110">Permission type</span></span>      | <span data-ttu-id="e149b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e149b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e149b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e149b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e149b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e149b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e149b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e149b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e149b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e149b-115">Not supported.</span></span>    |
|<span data-ttu-id="e149b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e149b-116">Application</span></span> | <span data-ttu-id="e149b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e149b-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e149b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e149b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="e149b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e149b-119">Request headers</span></span>
| <span data-ttu-id="e149b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e149b-120">Header</span></span>       | <span data-ttu-id="e149b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e149b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e149b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e149b-122">Authorization</span></span>  | <span data-ttu-id="e149b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e149b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e149b-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="e149b-125">Prefer</span></span> | <span data-ttu-id="e149b-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="e149b-126">return=minimal.</span></span> <span data-ttu-id="e149b-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e149b-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="e149b-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e149b-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="e149b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e149b-129">Request body</span></span>
 <span data-ttu-id="e149b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e149b-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="e149b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e149b-131">Response</span></span>
<span data-ttu-id="e149b-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e149b-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e149b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e149b-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e149b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e149b-135">Request</span></span>
<span data-ttu-id="e149b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e149b-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e149b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e149b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="e149b-138">C#</span><span class="sxs-lookup"><span data-stu-id="e149b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e149b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e149b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e149b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e149b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e149b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e149b-141">Response</span></span>
<span data-ttu-id="e149b-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e149b-142">The following is an example of the response.</span></span> 
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
