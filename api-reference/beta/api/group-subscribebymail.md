---
title: 'group: subscribeByMail'
description: С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе. Поддерживается только для групп Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bc87c2fbc7bab8ffd108abe54a89565e94c930f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418225"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="191b3-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="191b3-104">group: subscribeByMail</span></span>

<span data-ttu-id="191b3-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="191b3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="191b3-106">С помощью этого метода можно разрешить текущему пользователю получать уведомления электронной почты о новых записях, событиях и файлов в этой группе.</span><span class="sxs-lookup"><span data-stu-id="191b3-106">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="191b3-107">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="191b3-107">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="191b3-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="191b3-108">Permissions</span></span>
<span data-ttu-id="191b3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="191b3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="191b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="191b3-111">Permission type</span></span>      | <span data-ttu-id="191b3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="191b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="191b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="191b3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="191b3-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="191b3-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="191b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="191b3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="191b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b3-116">Not supported.</span></span>    |
|<span data-ttu-id="191b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="191b3-117">Application</span></span> | <span data-ttu-id="191b3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="191b3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="191b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="191b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="191b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="191b3-120">Request headers</span></span>
| <span data-ttu-id="191b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="191b3-121">Header</span></span>       | <span data-ttu-id="191b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="191b3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="191b3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="191b3-123">Authorization</span></span>  | <span data-ttu-id="191b3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="191b3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="191b3-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="191b3-126">Prefer</span></span> | <span data-ttu-id="191b3-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="191b3-127">return=minimal.</span></span> <span data-ttu-id="191b3-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="191b3-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="191b3-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="191b3-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="191b3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="191b3-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="191b3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b3-131">Response</span></span>
<span data-ttu-id="191b3-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="191b3-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="191b3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="191b3-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="191b3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="191b3-135">Request</span></span>
<span data-ttu-id="191b3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="191b3-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="191b3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="191b3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="191b3-138">C#</span><span class="sxs-lookup"><span data-stu-id="191b3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="191b3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="191b3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="191b3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="191b3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="191b3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="191b3-141">Response</span></span>
<span data-ttu-id="191b3-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="191b3-142">The following is an example of the response.</span></span> 
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
