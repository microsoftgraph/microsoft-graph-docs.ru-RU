---
title: Список Воркбуккомментс
description: Получение списка объектов Воркбуккомментс.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0571742da745831421d33088d67d1847796ddfd8
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838900"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="98602-103">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="98602-103">List workbookComments</span></span>

<span data-ttu-id="98602-104">Получение списка объектов [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="98602-104">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="98602-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98602-105">Permissions</span></span>

<span data-ttu-id="98602-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98602-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98602-108">Permission type</span></span>                        | <span data-ttu-id="98602-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98602-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98602-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98602-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98602-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98602-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="98602-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98602-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98602-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98602-113">Not supported.</span></span> |
| <span data-ttu-id="98602-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98602-114">Application</span></span>                            | <span data-ttu-id="98602-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98602-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98602-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98602-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="98602-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98602-117">Request headers</span></span>

| <span data-ttu-id="98602-118">Имя</span><span class="sxs-lookup"><span data-stu-id="98602-118">Name</span></span>      |<span data-ttu-id="98602-119">Описание</span><span class="sxs-lookup"><span data-stu-id="98602-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98602-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98602-120">Authorization</span></span> | <span data-ttu-id="98602-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98602-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98602-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98602-123">Request body</span></span>

<span data-ttu-id="98602-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98602-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98602-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="98602-125">Response</span></span>

<span data-ttu-id="98602-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98602-126">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98602-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="98602-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98602-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="98602-128">Request</span></span>

<span data-ttu-id="98602-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98602-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98602-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="98602-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/comments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98602-131">C#</span><span class="sxs-lookup"><span data-stu-id="98602-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98602-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98602-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98602-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="98602-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98602-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="98602-134">Response</span></span>

<span data-ttu-id="98602-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98602-135">The following is an example of the response.</span></span>

> <span data-ttu-id="98602-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98602-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
