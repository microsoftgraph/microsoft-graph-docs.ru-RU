---
title: Get workbookCommentReply
description: Извлечение свойств и связей объекта workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 10dcaca364a20120a2af86c9b300051b6c29d807
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049550"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="7d317-103">Get workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="7d317-103">Get workbookCommentReply</span></span>

<span data-ttu-id="7d317-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d317-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d317-105">Извлечение свойств и связей [объекта workbookCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="7d317-105">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d317-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d317-106">Permissions</span></span>

<span data-ttu-id="7d317-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d317-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d317-109">Permission type</span></span>                        | <span data-ttu-id="7d317-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d317-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7d317-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d317-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d317-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d317-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="7d317-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d317-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d317-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d317-114">Not supported.</span></span> |
| <span data-ttu-id="7d317-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d317-115">Application</span></span>                            | <span data-ttu-id="7d317-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d317-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d317-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d317-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{id}/workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7d317-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d317-118">Request headers</span></span>

| <span data-ttu-id="7d317-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d317-119">Name</span></span>      |<span data-ttu-id="7d317-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d317-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d317-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d317-121">Authorization</span></span> | <span data-ttu-id="7d317-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d317-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d317-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d317-124">Request body</span></span>

<span data-ttu-id="7d317-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d317-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d317-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d317-126">Response</span></span>

<span data-ttu-id="7d317-127">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [workbookCommentReply](../resources/workbookcommentreply.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d317-127">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d317-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d317-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d317-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d317-129">Request</span></span>

<span data-ttu-id="7d317-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d317-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d317-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d317-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies/{id}
```
# <a name="c"></a>[<span data-ttu-id="7d317-132">C#</span><span class="sxs-lookup"><span data-stu-id="7d317-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcommentreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d317-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d317-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcommentreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d317-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d317-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcommentreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d317-135">Java</span><span class="sxs-lookup"><span data-stu-id="7d317-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcommentreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7d317-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d317-136">Response</span></span>

<span data-ttu-id="7d317-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d317-137">The following is an example of the response.</span></span>

> <span data-ttu-id="7d317-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d317-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is text of comment.",
  "contentType": "Plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


