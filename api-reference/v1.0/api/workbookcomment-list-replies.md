---
title: Список книгCommentReplies
description: Извлечение списка объектов workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: faa089c24e6e332ad6da285400ffa11be2c6b2cd
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577662"
---
# <a name="list-workbookcommentreplies"></a><span data-ttu-id="0fb96-103">Список книгCommentReplies</span><span class="sxs-lookup"><span data-stu-id="0fb96-103">List workbookCommentReplies</span></span>

<span data-ttu-id="0fb96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fb96-105">Извлечение списка [объектов книгиCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="0fb96-105">Retrieve a list of [workbookCommentReply](../resources/workbookcommentreply.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fb96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fb96-106">Permissions</span></span>

<span data-ttu-id="0fb96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fb96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fb96-109">Permission type</span></span>                        | <span data-ttu-id="0fb96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fb96-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0fb96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fb96-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fb96-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fb96-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="0fb96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fb96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fb96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb96-114">Not supported.</span></span> |
| <span data-ttu-id="0fb96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fb96-115">Application</span></span>                            | <span data-ttu-id="0fb96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb96-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fb96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fb96-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}/replies
GET /me/drive/root:/{item-path}:/workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="0fb96-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fb96-118">Request headers</span></span>

| <span data-ttu-id="0fb96-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0fb96-119">Name</span></span>      |<span data-ttu-id="0fb96-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0fb96-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fb96-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fb96-121">Authorization</span></span> | <span data-ttu-id="0fb96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fb96-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fb96-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fb96-124">Request body</span></span>

<span data-ttu-id="0fb96-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fb96-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fb96-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb96-126">Response</span></span>

<span data-ttu-id="0fb96-127">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [workbookCommentReply](../resources/workbookcommentreply.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0fb96-127">If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fb96-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0fb96-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fb96-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fb96-129">Request</span></span>

<span data-ttu-id="0fb96-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fb96-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fb96-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb96-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}/replies
```
# <a name="c"></a>[<span data-ttu-id="0fb96-132">C#</span><span class="sxs-lookup"><span data-stu-id="0fb96-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fb96-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fb96-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fb96-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fb96-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fb96-135">Java</span><span class="sxs-lookup"><span data-stu-id="0fb96-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fb96-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb96-136">Response</span></span>

<span data-ttu-id="0fb96-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0fb96-137">The following is an example of the response.</span></span>

> <span data-ttu-id="0fb96-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fb96-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

