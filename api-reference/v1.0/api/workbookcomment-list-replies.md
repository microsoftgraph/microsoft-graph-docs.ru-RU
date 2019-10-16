---
title: Список Воркбуккомментреплиес
description: Получение списка объектов воркбуккомментрепли.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f2843f068bf8abb7612afdc0a21b68234324e52b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538667"
---
# <a name="list-workbookcommentreplies"></a><span data-ttu-id="23c59-103">Список Воркбуккомментреплиес</span><span class="sxs-lookup"><span data-stu-id="23c59-103">List workbookCommentReplies</span></span>

<span data-ttu-id="23c59-104">Получение списка объектов [воркбуккомментрепли](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="23c59-104">Retrieve a list of [workbookCommentReply](../resources/workbookcommentreply.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="23c59-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23c59-105">Permissions</span></span>

<span data-ttu-id="23c59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23c59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23c59-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23c59-108">Permission type</span></span>                        | <span data-ttu-id="23c59-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23c59-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23c59-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23c59-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23c59-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23c59-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="23c59-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23c59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c59-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23c59-113">Not supported.</span></span> |
| <span data-ttu-id="23c59-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23c59-114">Application</span></span>                            | <span data-ttu-id="23c59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23c59-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23c59-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23c59-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="23c59-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23c59-117">Request headers</span></span>

| <span data-ttu-id="23c59-118">Имя</span><span class="sxs-lookup"><span data-stu-id="23c59-118">Name</span></span>      |<span data-ttu-id="23c59-119">Описание</span><span class="sxs-lookup"><span data-stu-id="23c59-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23c59-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23c59-120">Authorization</span></span> | <span data-ttu-id="23c59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23c59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c59-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23c59-123">Request body</span></span>

<span data-ttu-id="23c59-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23c59-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23c59-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="23c59-125">Response</span></span>

<span data-ttu-id="23c59-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуккомментрепли](../resources/workbookcommentreply.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23c59-126">If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23c59-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="23c59-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23c59-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="23c59-128">Request</span></span>

<span data-ttu-id="23c59-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23c59-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23c59-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="23c59-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_replies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23c59-131">C#</span><span class="sxs-lookup"><span data-stu-id="23c59-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23c59-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23c59-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23c59-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23c59-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23c59-134">Java</span><span class="sxs-lookup"><span data-stu-id="23c59-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-replies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23c59-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="23c59-135">Response</span></span>

<span data-ttu-id="23c59-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23c59-136">The following is an example of the response.</span></span>

> <span data-ttu-id="23c59-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23c59-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
