---
title: Список книгCommentReplies
description: Извлечение списка объектов книгиCommentReplies.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0c3e96d13266b294f51105bbdd4437cb526f3a33
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049564"
---
# <a name="list-workbookcommentreplies"></a><span data-ttu-id="395c5-103">Список книгCommentReplies</span><span class="sxs-lookup"><span data-stu-id="395c5-103">List workbookCommentReplies</span></span>

<span data-ttu-id="395c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="395c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="395c5-105">Извлечение списка [объектов книгиCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="395c5-105">Retrieve a list of [workbookCommentReply](../resources/workbookcommentreply.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="395c5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="395c5-106">Permissions</span></span>

<span data-ttu-id="395c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="395c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="395c5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="395c5-109">Permission type</span></span>                        | <span data-ttu-id="395c5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="395c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="395c5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="395c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="395c5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="395c5-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="395c5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="395c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="395c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395c5-114">Not supported.</span></span> |
| <span data-ttu-id="395c5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="395c5-115">Application</span></span>                            | <span data-ttu-id="395c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395c5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="395c5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="395c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}/replies
GET /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="395c5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="395c5-118">Request headers</span></span>

| <span data-ttu-id="395c5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="395c5-119">Name</span></span>      |<span data-ttu-id="395c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="395c5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="395c5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="395c5-121">Authorization</span></span> | <span data-ttu-id="395c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="395c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="395c5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="395c5-124">Request body</span></span>

<span data-ttu-id="395c5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="395c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="395c5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="395c5-126">Response</span></span>

<span data-ttu-id="395c5-127">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [workbookCommentReply](../resources/workbookcommentreply.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="395c5-127">If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="395c5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="395c5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="395c5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="395c5-129">Request</span></span>

<span data-ttu-id="395c5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="395c5-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="395c5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="395c5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="395c5-132">C#</span><span class="sxs-lookup"><span data-stu-id="395c5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="395c5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="395c5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="395c5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="395c5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="395c5-135">Java</span><span class="sxs-lookup"><span data-stu-id="395c5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="395c5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="395c5-136">Response</span></span>

<span data-ttu-id="395c5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="395c5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="395c5-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="395c5-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is the first piece of reply.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}" 
    },
    {
      "content": "This is the second piece of reply.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFF9}"
     }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


