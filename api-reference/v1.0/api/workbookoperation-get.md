---
title: Get workbookOperation
description: Извлечение состояния объекта workbookOperation.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5947f24447a96d4f28275322b25b507c95256978
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626140"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="875c0-103">Get workbookOperation</span><span class="sxs-lookup"><span data-stu-id="875c0-103">Get workbookOperation</span></span>

<span data-ttu-id="875c0-104">Извлечение состояния [объекта workbookOperation.](../resources/workbookoperation.md)</span><span class="sxs-lookup"><span data-stu-id="875c0-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="875c0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="875c0-105">Permissions</span></span>

<span data-ttu-id="875c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="875c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="875c0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="875c0-108">Permission type</span></span>                        | <span data-ttu-id="875c0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="875c0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="875c0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="875c0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="875c0-111">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="875c0-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="875c0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="875c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="875c0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="875c0-113">Not supported.</span></span> |
| <span data-ttu-id="875c0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="875c0-114">Application</span></span>                            | <span data-ttu-id="875c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="875c0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="875c0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="875c0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/items/{id}/workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="875c0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="875c0-117">Request headers</span></span>

| <span data-ttu-id="875c0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="875c0-118">Name</span></span>      |<span data-ttu-id="875c0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="875c0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="875c0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="875c0-120">Authorization</span></span> | <span data-ttu-id="875c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="875c0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="875c0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="875c0-123">Request body</span></span>

<span data-ttu-id="875c0-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="875c0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="875c0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="875c0-125">Response</span></span>

<span data-ttu-id="875c0-126">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [workbookOperation](../resources/workbookoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="875c0-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="875c0-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="875c0-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="875c0-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="875c0-128">Request</span></span>

<span data-ttu-id="875c0-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="875c0-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="875c0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="875c0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="875c0-131">C#</span><span class="sxs-lookup"><span data-stu-id="875c0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="875c0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="875c0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="875c0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="875c0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="875c0-134">Java</span><span class="sxs-lookup"><span data-stu-id="875c0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="875c0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="875c0-135">Response</span></span>

<span data-ttu-id="875c0-136">Ниже приводится ответ со статусом "запуск".</span><span class="sxs-lookup"><span data-stu-id="875c0-136">The following is the response with the status of "running".</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "running"
}
```

<span data-ttu-id="875c0-137">Ниже приводится ответ со статусом "успешно".</span><span class="sxs-lookup"><span data-stu-id="875c0-137">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="875c0-138">Ниже приводится ответ со статусом "не удалось".</span><span class="sxs-lookup"><span data-stu-id="875c0-138">The following is the response with the status of "failed".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "failed",
  "error":
  {
      "code": "internalServerError",
      "message": "An internal server error occurred while processing the request.",
      "innerError": {
          "code": ""internalServerErrorUncategorized",
          "message": "An unspecified error has occurred.",
          "innerError": {
               "code": "GenericFileOpenError",
               "message": "The workbook cannot be opened."
          }
      }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

