---
title: Get workbookCommentReply
description: Извлечение свойств и связей объекта workbookcommentreply.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 48a93ff5828a8dcba909acf74fbfca9582d2cf95
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578719"
---
# <a name="get-workbookcommentreply"></a><span data-ttu-id="b5e85-103">Get workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="b5e85-103">Get workbookCommentReply</span></span>

<span data-ttu-id="b5e85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e85-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5e85-105">Извлечение свойств и связей [объекта workbookCommentReply.](../resources/workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="b5e85-105">Retrieve the properties and relationships of [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e85-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5e85-106">Permissions</span></span>

<span data-ttu-id="b5e85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5e85-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5e85-109">Permission type</span></span>                        | <span data-ttu-id="b5e85-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5e85-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5e85-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5e85-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5e85-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e85-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="b5e85-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5e85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e85-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5e85-114">Not supported.</span></span> |
| <span data-ttu-id="b5e85-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5e85-115">Application</span></span>                            | <span data-ttu-id="b5e85-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5e85-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e85-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5e85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}/replies/{id}
GET /me/drive/root:/{item-path}:/workbook/comments/{id}/replies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5e85-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5e85-118">Request headers</span></span>

| <span data-ttu-id="b5e85-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b5e85-119">Name</span></span>      |<span data-ttu-id="b5e85-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b5e85-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5e85-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5e85-121">Authorization</span></span> | <span data-ttu-id="b5e85-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5e85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e85-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5e85-124">Request body</span></span>

<span data-ttu-id="b5e85-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5e85-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e85-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e85-126">Response</span></span>

<span data-ttu-id="b5e85-127">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [workbookCommentReply](../resources/workbookcommentreply.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b5e85-127">If successful, this method returns a `200 OK` response code and the requested [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5e85-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5e85-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5e85-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5e85-129">Request</span></span>

<span data-ttu-id="b5e85-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5e85-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5e85-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e85-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}/replies/{id}
```
# <a name="c"></a>[<span data-ttu-id="b5e85-132">C#</span><span class="sxs-lookup"><span data-stu-id="b5e85-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcommentreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e85-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e85-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcommentreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e85-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e85-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcommentreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e85-135">Java</span><span class="sxs-lookup"><span data-stu-id="b5e85-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcommentreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5e85-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e85-136">Response</span></span>

<span data-ttu-id="b5e85-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5e85-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b5e85-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5e85-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

