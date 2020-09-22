---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d6242084d73f3b53da79b1fd768105f4d05c812e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001997"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="a65b7-103">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="a65b7-103">group: subscribeByMail</span></span>

<span data-ttu-id="a65b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a65b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a65b7-105">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="a65b7-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="a65b7-106">Поддерживается только для групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a65b7-106">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="a65b7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a65b7-107">Permissions</span></span>
<span data-ttu-id="a65b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a65b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a65b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a65b7-110">Permission type</span></span>      | <span data-ttu-id="a65b7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a65b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a65b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a65b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a65b7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a65b7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a65b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a65b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a65b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65b7-115">Not supported.</span></span>    |
|<span data-ttu-id="a65b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a65b7-116">Application</span></span> | <span data-ttu-id="a65b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a65b7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a65b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a65b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="a65b7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a65b7-119">Request headers</span></span>
| <span data-ttu-id="a65b7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a65b7-120">Header</span></span>       | <span data-ttu-id="a65b7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a65b7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a65b7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a65b7-122">Authorization</span></span>  | <span data-ttu-id="a65b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a65b7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a65b7-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="a65b7-125">Prefer</span></span> | <span data-ttu-id="a65b7-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="a65b7-126">return=minimal.</span></span> <span data-ttu-id="a65b7-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a65b7-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="a65b7-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a65b7-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a65b7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a65b7-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a65b7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65b7-130">Response</span></span>
<span data-ttu-id="a65b7-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a65b7-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a65b7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a65b7-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a65b7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a65b7-134">Request</span></span>
<span data-ttu-id="a65b7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a65b7-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a65b7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a65b7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="a65b7-137">C#</span><span class="sxs-lookup"><span data-stu-id="a65b7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a65b7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a65b7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a65b7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a65b7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a65b7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a65b7-140">Response</span></span>
<span data-ttu-id="a65b7-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a65b7-141">The following is an example of the response.</span></span> 
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


