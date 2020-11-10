---
title: Получение Воркбуккоммент
description: Получение свойств и связей объекта воркбуккоммент.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a80122caee0d6b04b24b0a1e4c60818f0ef7bea5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977508"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="5bb5d-103">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="5bb5d-103">Get workbookComment</span></span>

<span data-ttu-id="5bb5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bb5d-105">Получение свойств и связей объекта [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="5bb5d-105">Get the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bb5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bb5d-106">Permissions</span></span>

<span data-ttu-id="5bb5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bb5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bb5d-109">Permission type</span></span>                        | <span data-ttu-id="5bb5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5bb5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bb5d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bb5d-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="5bb5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bb5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-114">Not supported.</span></span> |
| <span data-ttu-id="5bb5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bb5d-115">Application</span></span>                            | <span data-ttu-id="5bb5d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bb5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bb5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5bb5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bb5d-118">Request headers</span></span>

| <span data-ttu-id="5bb5d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5bb5d-119">Name</span></span>      |<span data-ttu-id="5bb5d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5bb5d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bb5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bb5d-121">Authorization</span></span> | <span data-ttu-id="5bb5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bb5d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bb5d-124">Request body</span></span>

<span data-ttu-id="5bb5d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bb5d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb5d-126">Response</span></span>

<span data-ttu-id="5bb5d-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-127">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bb5d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5bb5d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bb5d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bb5d-129">Request</span></span>

<span data-ttu-id="5bb5d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5bb5d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb5d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}
```
# <a name="c"></a>[<span data-ttu-id="5bb5d-132">C#</span><span class="sxs-lookup"><span data-stu-id="5bb5d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bb5d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bb5d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bb5d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bb5d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bb5d-135">Java</span><span class="sxs-lookup"><span data-stu-id="5bb5d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bb5d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb5d-136">Response</span></span>

<span data-ttu-id="5bb5d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="5bb5d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


