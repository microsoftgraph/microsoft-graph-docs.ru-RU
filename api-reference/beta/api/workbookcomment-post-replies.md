---
title: Создание книгиCommentReply
description: Создание новой книгиCommentReply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cfa09de241b74bb9bd1a3289791564a9edac5128
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049557"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="f3024-103">Создание книгиCommentReply</span><span class="sxs-lookup"><span data-stu-id="f3024-103">Create workbookCommentReply</span></span>

<span data-ttu-id="f3024-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3024-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3024-105">Создайте новый [объект книгиCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="f3024-105">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3024-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3024-106">Permissions</span></span>

<span data-ttu-id="f3024-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3024-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3024-109">Permission type</span></span>                        | <span data-ttu-id="f3024-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3024-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f3024-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3024-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3024-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3024-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="f3024-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3024-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3024-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3024-114">Not supported.</span></span> |
| <span data-ttu-id="f3024-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3024-115">Application</span></span>                            | <span data-ttu-id="f3024-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3024-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3024-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3024-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{id}/workbook/comments/{id}/replies
POST /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="f3024-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3024-118">Request headers</span></span>

| <span data-ttu-id="f3024-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f3024-119">Name</span></span>          | <span data-ttu-id="f3024-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f3024-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f3024-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3024-121">Authorization</span></span> | <span data-ttu-id="f3024-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3024-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3024-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3024-124">Request body</span></span>

<span data-ttu-id="f3024-125">В теле запроса поставляем представление JSON объекта [книгиCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="f3024-125">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3024-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3024-126">Response</span></span>

<span data-ttu-id="f3024-127">В случае успешного выполнения этот метод возвращает код отклика и новый объект `201 Created` [workbookCommentReply](../resources/workbookcommentreply.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3024-127">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3024-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f3024-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3024-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3024-129">Request</span></span>

<span data-ttu-id="f3024-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3024-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3024-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3024-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="c"></a>[<span data-ttu-id="f3024-132">C#</span><span class="sxs-lookup"><span data-stu-id="f3024-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3024-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3024-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3024-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3024-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3024-135">Java</span><span class="sxs-lookup"><span data-stu-id="f3024-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3024-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3024-136">Response</span></span>

<span data-ttu-id="f3024-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f3024-137">The following is an example of the response.</span></span>

> <span data-ttu-id="f3024-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f3024-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


