---
title: 'group: unsubscribeByMail'
description: 'Вызов этого метода отключит текущего пользователя на получение уведомлений по электронной почте для этой группы о новых публикациях, событиях и файлах в этой группе. Поддерживается только для групп Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 252fd8fbcc878c7d77818e2215cd8a06ea4722b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418237"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="c2a6b-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="c2a6b-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="c2a6b-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2a6b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2a6b-106">Вызов этого метода отключит текущего пользователя на получение уведомлений по электронной почте для этой группы о новых публикациях, событиях и файлах в этой группе.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-106">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="c2a6b-107">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-107">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c2a6b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2a6b-108">Permissions</span></span>
<span data-ttu-id="c2a6b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2a6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2a6b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2a6b-111">Permission type</span></span>      | <span data-ttu-id="c2a6b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2a6b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2a6b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2a6b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c2a6b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a6b-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2a6b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2a6b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2a6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-116">Not supported.</span></span>    |
|<span data-ttu-id="c2a6b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2a6b-117">Application</span></span> | <span data-ttu-id="c2a6b-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a6b-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2a6b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2a6b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="c2a6b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2a6b-120">Request headers</span></span>
| <span data-ttu-id="c2a6b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2a6b-121">Header</span></span>       | <span data-ttu-id="c2a6b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2a6b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2a6b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2a6b-123">Authorization</span></span>  | <span data-ttu-id="c2a6b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2a6b-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="c2a6b-126">Prefer</span></span> | <span data-ttu-id="c2a6b-127">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-127">return=minimal.</span></span> <span data-ttu-id="c2a6b-128">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="c2a6b-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="c2a6b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2a6b-130">Request body</span></span>
 <span data-ttu-id="c2a6b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="c2a6b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2a6b-132">Response</span></span>
<span data-ttu-id="c2a6b-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2a6b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c2a6b-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c2a6b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2a6b-136">Request</span></span>
<span data-ttu-id="c2a6b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2a6b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2a6b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="c2a6b-139">C#</span><span class="sxs-lookup"><span data-stu-id="c2a6b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2a6b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2a6b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2a6b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2a6b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2a6b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2a6b-142">Response</span></span>
<span data-ttu-id="c2a6b-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2a6b-143">The following is an example of the response.</span></span> 
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
