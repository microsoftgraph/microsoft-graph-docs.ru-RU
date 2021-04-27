---
title: Get workbookComment
description: Получите свойства и связи объекта книги.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 132925396dd9f8e9acebfd2192b58d090d6d80b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049571"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="098fd-103">Get workbookComment</span><span class="sxs-lookup"><span data-stu-id="098fd-103">Get workbookComment</span></span>

<span data-ttu-id="098fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="098fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="098fd-105">Получите свойства и связи объекта [workbookComment.](../resources/workbookcomment.md)</span><span class="sxs-lookup"><span data-stu-id="098fd-105">Get the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="098fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="098fd-106">Permissions</span></span>

<span data-ttu-id="098fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="098fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="098fd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="098fd-109">Permission type</span></span>                        | <span data-ttu-id="098fd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="098fd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="098fd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="098fd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="098fd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="098fd-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="098fd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="098fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="098fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="098fd-114">Not supported.</span></span> |
| <span data-ttu-id="098fd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="098fd-115">Application</span></span>                            | <span data-ttu-id="098fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="098fd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="098fd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="098fd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="098fd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="098fd-118">Request headers</span></span>

| <span data-ttu-id="098fd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="098fd-119">Name</span></span>      |<span data-ttu-id="098fd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="098fd-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="098fd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="098fd-121">Authorization</span></span> | <span data-ttu-id="098fd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="098fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="098fd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="098fd-124">Request body</span></span>

<span data-ttu-id="098fd-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="098fd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="098fd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="098fd-126">Response</span></span>

<span data-ttu-id="098fd-127">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [workbookComment](../resources/workbookcomment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="098fd-127">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="098fd-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="098fd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="098fd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="098fd-129">Request</span></span>

<span data-ttu-id="098fd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="098fd-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="098fd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="098fd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}
```
# <a name="c"></a>[<span data-ttu-id="098fd-132">C#</span><span class="sxs-lookup"><span data-stu-id="098fd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="098fd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="098fd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="098fd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="098fd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="098fd-135">Java</span><span class="sxs-lookup"><span data-stu-id="098fd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="098fd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="098fd-136">Response</span></span>

<span data-ttu-id="098fd-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="098fd-137">The following is an example of the response.</span></span>

> <span data-ttu-id="098fd-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="098fd-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is my comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookComment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


