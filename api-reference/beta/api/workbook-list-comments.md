---
title: Список книгКомменты
description: Извлечение списка объектов workbookComments.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d704ee34d54c2b4369b544f8886f69fc6286e15b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036169"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="7fec3-103">Список книгКомменты</span><span class="sxs-lookup"><span data-stu-id="7fec3-103">List workbookComments</span></span>

<span data-ttu-id="7fec3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fec3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fec3-105">Извлечение списка [объектов книгиComment.](../resources/workbookcomment.md)</span><span class="sxs-lookup"><span data-stu-id="7fec3-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fec3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fec3-106">Permissions</span></span>

<span data-ttu-id="7fec3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fec3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fec3-109">Permission type</span></span>                        | <span data-ttu-id="7fec3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fec3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7fec3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fec3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fec3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fec3-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="7fec3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fec3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fec3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fec3-114">Not supported.</span></span> |
| <span data-ttu-id="7fec3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fec3-115">Application</span></span>                            | <span data-ttu-id="7fec3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fec3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fec3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fec3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments
GET /me/drive/root:/{item-path}:/workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="7fec3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fec3-118">Request headers</span></span>

| <span data-ttu-id="7fec3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7fec3-119">Name</span></span>      |<span data-ttu-id="7fec3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7fec3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fec3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fec3-121">Authorization</span></span> | <span data-ttu-id="7fec3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fec3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fec3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fec3-124">Request body</span></span>

<span data-ttu-id="7fec3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fec3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fec3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fec3-126">Response</span></span>

<span data-ttu-id="7fec3-127">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [workbookComment](../resources/workbookcomment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7fec3-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fec3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7fec3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fec3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fec3-129">Request</span></span>

<span data-ttu-id="7fec3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fec3-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fec3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fec3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="7fec3-132">C#</span><span class="sxs-lookup"><span data-stu-id="7fec3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fec3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fec3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fec3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fec3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fec3-135">Java</span><span class="sxs-lookup"><span data-stu-id="7fec3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-comments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fec3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fec3-136">Response</span></span>

<span data-ttu-id="7fec3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7fec3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="7fec3-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7fec3-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "content": "This is text of comment.",
      "contentType": "plain",
      "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List comments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


