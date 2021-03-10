---
title: Get workbookComment
description: Получите свойства и связи объекта книги.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5355a52998e0f3e2f61fa2834bf3e482669a1f56
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626211"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="92fe5-103">Get workbookComment</span><span class="sxs-lookup"><span data-stu-id="92fe5-103">Get workbookComment</span></span>

<span data-ttu-id="92fe5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92fe5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92fe5-105">Получите свойства и связи объекта [workbookComment.](../resources/workbookcomment.md)</span><span class="sxs-lookup"><span data-stu-id="92fe5-105">Get the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92fe5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92fe5-106">Permissions</span></span>

<span data-ttu-id="92fe5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92fe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92fe5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92fe5-109">Permission type</span></span>                        | <span data-ttu-id="92fe5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92fe5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92fe5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92fe5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92fe5-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92fe5-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="92fe5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92fe5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92fe5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92fe5-114">Not supported.</span></span> |
| <span data-ttu-id="92fe5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92fe5-115">Application</span></span>                            | <span data-ttu-id="92fe5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92fe5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92fe5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92fe5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92fe5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92fe5-118">Request headers</span></span>

| <span data-ttu-id="92fe5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="92fe5-119">Name</span></span>      |<span data-ttu-id="92fe5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92fe5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92fe5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92fe5-121">Authorization</span></span> | <span data-ttu-id="92fe5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92fe5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92fe5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92fe5-124">Request body</span></span>

<span data-ttu-id="92fe5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92fe5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92fe5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="92fe5-126">Response</span></span>

<span data-ttu-id="92fe5-127">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [workbookComment](../resources/workbookcomment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="92fe5-127">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92fe5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="92fe5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92fe5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="92fe5-129">Request</span></span>

<span data-ttu-id="92fe5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92fe5-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92fe5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="92fe5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}
```
# <a name="c"></a>[<span data-ttu-id="92fe5-132">C#</span><span class="sxs-lookup"><span data-stu-id="92fe5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92fe5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92fe5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92fe5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92fe5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92fe5-135">Java</span><span class="sxs-lookup"><span data-stu-id="92fe5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92fe5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="92fe5-136">Response</span></span>

<span data-ttu-id="92fe5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92fe5-137">The following is an example of the response.</span></span>

> <span data-ttu-id="92fe5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92fe5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


