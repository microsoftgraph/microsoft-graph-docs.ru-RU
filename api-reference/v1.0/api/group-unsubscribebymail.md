---
title: 'group: unsubscribeByMail'
description: 'С помощью этого метода можно заблокировать для текущего пользователя получение уведомлений электронной почты о новых записях, событиях и файлах в этой группе. Поддерживается только для групп Office 365. '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cc0375efe70482c248fa5f9d3168e2562f9416a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516930"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="b2269-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b2269-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="b2269-105">Пространство имен: вызов Microsoft. Graph. Этот метод не позволит текущему пользователю получать уведомления по электронной почте для этой группы о новых сообщениях, событиях и файлах в этой группе.</span><span class="sxs-lookup"><span data-stu-id="b2269-105">Namespace: microsoft.graph Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="b2269-106">Поддерживается только для групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="b2269-106">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b2269-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2269-107">Permissions</span></span>
<span data-ttu-id="b2269-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2269-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2269-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2269-110">Permission type</span></span>      | <span data-ttu-id="b2269-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2269-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2269-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2269-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2269-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2269-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2269-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2269-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2269-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2269-115">Not supported.</span></span>    |
|<span data-ttu-id="b2269-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2269-116">Application</span></span> | <span data-ttu-id="b2269-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2269-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2269-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2269-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="b2269-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2269-119">Request headers</span></span>
| <span data-ttu-id="b2269-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2269-120">Header</span></span>       | <span data-ttu-id="b2269-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2269-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2269-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2269-122">Authorization</span></span>  | <span data-ttu-id="b2269-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2269-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b2269-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="b2269-125">Prefer</span></span> | <span data-ttu-id="b2269-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="b2269-126">return=minimal.</span></span> <span data-ttu-id="b2269-127">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b2269-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b2269-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b2269-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b2269-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2269-129">Request body</span></span>
<span data-ttu-id="b2269-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2269-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2269-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2269-131">Response</span></span>
<span data-ttu-id="b2269-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b2269-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2269-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b2269-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b2269-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2269-135">Request</span></span>
<span data-ttu-id="b2269-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2269-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2269-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2269-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="b2269-138">C#</span><span class="sxs-lookup"><span data-stu-id="b2269-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2269-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2269-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2269-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2269-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2269-141">Java</span><span class="sxs-lookup"><span data-stu-id="b2269-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b2269-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2269-142">Response</span></span>
<span data-ttu-id="b2269-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b2269-143">The following is an example of the response.</span></span> 
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
