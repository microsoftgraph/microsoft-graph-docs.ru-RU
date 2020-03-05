---
title: Список Воркбуккомментс
description: Получение списка объектов Воркбуккомментс.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4e7ecb65038dbc2e75c8642a3e2d3552f338e89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451485"
---
# <a name="list-workbookcomments"></a><span data-ttu-id="de957-103">Список Воркбуккомментс</span><span class="sxs-lookup"><span data-stu-id="de957-103">List workbookComments</span></span>

<span data-ttu-id="de957-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de957-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de957-105">Получение списка объектов [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="de957-105">Retrieve a list of  [workbookComment](../resources/workbookcomment.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="de957-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de957-106">Permissions</span></span>

<span data-ttu-id="de957-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de957-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de957-109">Permission type</span></span>                        | <span data-ttu-id="de957-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de957-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de957-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de957-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de957-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de957-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="de957-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de957-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de957-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de957-114">Not supported.</span></span> |
| <span data-ttu-id="de957-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de957-115">Application</span></span>                            | <span data-ttu-id="de957-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de957-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de957-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de957-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /workbook/comments
```

## <a name="request-headers"></a><span data-ttu-id="de957-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de957-118">Request headers</span></span>

| <span data-ttu-id="de957-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de957-119">Name</span></span>      |<span data-ttu-id="de957-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de957-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de957-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de957-121">Authorization</span></span> | <span data-ttu-id="de957-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de957-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de957-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de957-124">Request body</span></span>

<span data-ttu-id="de957-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de957-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de957-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="de957-126">Response</span></span>

<span data-ttu-id="de957-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de957-127">If successful, this method returns a `200 OK` response code and a collection of [workbookComment](../resources/workbookcomment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de957-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="de957-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de957-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="de957-129">Request</span></span>

<span data-ttu-id="de957-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de957-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de957-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="de957-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_comments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/comments
```
# <a name="c"></a>[<span data-ttu-id="de957-132">C#</span><span class="sxs-lookup"><span data-stu-id="de957-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-comments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de957-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de957-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-comments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de957-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de957-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-comments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de957-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="de957-135">Response</span></span>

<span data-ttu-id="de957-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de957-136">The following is an example of the response.</span></span>

> <span data-ttu-id="de957-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de957-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
