---
title: Удаление объекта acceptedSender
description: 'Удаление пользователя или группы из списка принятых отправителей. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1d867f3341ac6316354afa16b713e1961867b7bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023340"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="1c97a-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="1c97a-103">Remove acceptedSender</span></span>

<span data-ttu-id="1c97a-104">Пространство имен: Microsoft. Graph удаление пользователя или группы из списка принятых отправителей.</span><span class="sxs-lookup"><span data-stu-id="1c97a-104">Namespace: microsoft.graph Remove a user or group from the accepted-senders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1c97a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c97a-105">Permissions</span></span>
<span data-ttu-id="1c97a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c97a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c97a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c97a-108">Permission type</span></span>                        | <span data-ttu-id="1c97a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c97a-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="1c97a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c97a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c97a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c97a-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1c97a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c97a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c97a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c97a-113">Not supported.</span></span> |
| <span data-ttu-id="1c97a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c97a-114">Application</span></span>                            | <span data-ttu-id="1c97a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c97a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c97a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c97a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="1c97a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c97a-117">Request headers</span></span>
| <span data-ttu-id="1c97a-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c97a-118">Header</span></span>         | <span data-ttu-id="1c97a-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1c97a-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="1c97a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c97a-120">Authorization</span></span>  | <span data-ttu-id="1c97a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c97a-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="1c97a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c97a-123">Request body</span></span>
<span data-ttu-id="1c97a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c97a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c97a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c97a-125">Response</span></span>
<span data-ttu-id="1c97a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1c97a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c97a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1c97a-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1c97a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c97a-129">Request</span></span>
<span data-ttu-id="1c97a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c97a-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c97a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c97a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_acceptedsenders_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="1c97a-132">C#</span><span class="sxs-lookup"><span data-stu-id="1c97a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-acceptedsenders-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c97a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c97a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-acceptedsenders-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c97a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c97a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-acceptedsenders-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c97a-135">Java</span><span class="sxs-lookup"><span data-stu-id="1c97a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-acceptedsenders-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1c97a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c97a-136">Response</span></span>
<span data-ttu-id="1c97a-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c97a-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

