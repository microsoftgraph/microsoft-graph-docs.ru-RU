---
title: Получение Воркбукоператион
description: Получение свойств и связей объекта Воркбукоператион.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c5ead367116603a286574a30551134f9176d1477
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566188"
---
# <a name="get-workbookoperation"></a><span data-ttu-id="5465e-103">Получение Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="5465e-103">Get workbookOperation</span></span>

<span data-ttu-id="5465e-104">Получение состояния объекта [воркбукоператион](../resources/workbookoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="5465e-104">Retrieve the status of a [workbookOperation](../resources/workbookoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5465e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5465e-105">Permissions</span></span>

<span data-ttu-id="5465e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5465e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5465e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5465e-108">Permission type</span></span>                        | <span data-ttu-id="5465e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5465e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5465e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5465e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5465e-111">Files. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="5465e-111">Files.ReadWrite.</span></span> |
| <span data-ttu-id="5465e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5465e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5465e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5465e-113">Not supported.</span></span> |
| <span data-ttu-id="5465e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5465e-114">Application</span></span>                            | <span data-ttu-id="5465e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5465e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5465e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5465e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="5465e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5465e-117">Request headers</span></span>

| <span data-ttu-id="5465e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5465e-118">Name</span></span>      |<span data-ttu-id="5465e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5465e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5465e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5465e-120">Authorization</span></span> | <span data-ttu-id="5465e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5465e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5465e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5465e-123">Request body</span></span>

<span data-ttu-id="5465e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5465e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5465e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5465e-125">Response</span></span>

<span data-ttu-id="5465e-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркбукоператион](../resources/workbookoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5465e-126">If successful, this method returns a `200 OK` response code and the requested [workbookOperation](../resources/workbookoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5465e-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="5465e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5465e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="5465e-128">Request</span></span>

<span data-ttu-id="5465e-129">Ниже приведен пример запроса длительного выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="5465e-129">The following is an example of a long-running operation request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5465e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5465e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```
# <a name="c"></a>[<span data-ttu-id="5465e-131">C#</span><span class="sxs-lookup"><span data-stu-id="5465e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5465e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5465e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5465e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5465e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5465e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5465e-134">Response</span></span>

<span data-ttu-id="5465e-135">Ниже приведен ответ со статусом "работает".</span><span class="sxs-lookup"><span data-stu-id="5465e-135">The following is the response with the status of "running".</span></span>


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

<span data-ttu-id="5465e-136">Ниже приведен ответ со статусом "выполнено успешно".</span><span class="sxs-lookup"><span data-stu-id="5465e-136">The following is the response with the status of "succeeded".</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/beta/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

<span data-ttu-id="5465e-137">Ниже приведен ответ со статусом "Failed".</span><span class="sxs-lookup"><span data-stu-id="5465e-137">The following is the response with the status of "failed".</span></span>

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
