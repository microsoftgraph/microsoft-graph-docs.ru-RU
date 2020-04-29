---
title: Получение Воркбуккоммент
description: Получение свойств и связей объекта воркбуккоммент.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7e0a59c3c8c6deceb28aadd6fbc58e18ace0e5b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508816"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="9e8fe-103">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="9e8fe-103">Get workbookComment</span></span>

<span data-ttu-id="9e8fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e8fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e8fe-105">Получение свойств и связей объекта [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="9e8fe-105">Retrieve the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e8fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e8fe-106">Permissions</span></span>

<span data-ttu-id="9e8fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e8fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e8fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e8fe-109">Permission type</span></span>                        | <span data-ttu-id="9e8fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e8fe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e8fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e8fe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e8fe-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e8fe-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="9e8fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e8fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e8fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-114">Not supported.</span></span> |
| <span data-ttu-id="9e8fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e8fe-115">Application</span></span>                            | <span data-ttu-id="9e8fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e8fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e8fe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9e8fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e8fe-118">Request headers</span></span>

| <span data-ttu-id="9e8fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9e8fe-119">Name</span></span>      |<span data-ttu-id="9e8fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9e8fe-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e8fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e8fe-121">Authorization</span></span> | <span data-ttu-id="9e8fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e8fe-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e8fe-124">Request body</span></span>

<span data-ttu-id="9e8fe-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e8fe-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e8fe-126">Response</span></span>

<span data-ttu-id="9e8fe-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-127">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e8fe-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9e8fe-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e8fe-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e8fe-129">Request</span></span>

<span data-ttu-id="9e8fe-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e8fe-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e8fe-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/items/{id}/workbook/comments/{id}
```
# <a name="c"></a>[<span data-ttu-id="9e8fe-132">C#</span><span class="sxs-lookup"><span data-stu-id="9e8fe-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e8fe-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e8fe-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e8fe-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e8fe-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e8fe-135">Java</span><span class="sxs-lookup"><span data-stu-id="9e8fe-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e8fe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e8fe-136">Response</span></span>

<span data-ttu-id="9e8fe-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9e8fe-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e8fe-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
