---
title: Список границ
description: Получение списка объектов rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 8a18e47527bee9530cf425c30098e77282715095
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411993"
---
# <a name="list-borders"></a><span data-ttu-id="efa40-103">Список границ</span><span class="sxs-lookup"><span data-stu-id="efa40-103">List borders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efa40-104">Получение списка объектов rangeborder.</span><span class="sxs-lookup"><span data-stu-id="efa40-104">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="efa40-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efa40-105">Permissions</span></span>
<span data-ttu-id="efa40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa40-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efa40-108">Permission type</span></span>      | <span data-ttu-id="efa40-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efa40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efa40-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efa40-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efa40-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efa40-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efa40-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efa40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efa40-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="efa40-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="efa40-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efa40-114">Application</span></span> | <span data-ttu-id="efa40-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efa40-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efa40-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efa40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efa40-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efa40-117">Optional query parameters</span></span>
<span data-ttu-id="efa40-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="efa40-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efa40-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efa40-119">Request headers</span></span>
| <span data-ttu-id="efa40-120">Имя</span><span class="sxs-lookup"><span data-stu-id="efa40-120">Name</span></span>      |<span data-ttu-id="efa40-121">Описание</span><span class="sxs-lookup"><span data-stu-id="efa40-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="efa40-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efa40-122">Authorization</span></span>  | <span data-ttu-id="efa40-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efa40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="efa40-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="efa40-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="efa40-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="efa40-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa40-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efa40-128">Request body</span></span>
<span data-ttu-id="efa40-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efa40-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efa40-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa40-130">Response</span></span>

<span data-ttu-id="efa40-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукранжебордер](../resources/workbookrangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efa40-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeBorder](../resources/workbookrangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efa40-132">Пример</span><span class="sxs-lookup"><span data-stu-id="efa40-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efa40-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="efa40-133">Request</span></span>
<span data-ttu-id="efa40-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efa40-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="efa40-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="efa40-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="efa40-136">C#</span><span class="sxs-lookup"><span data-stu-id="efa40-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-borders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="efa40-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efa40-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-borders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="efa40-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="efa40-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-borders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="efa40-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="efa40-139">Response</span></span>
<span data-ttu-id="efa40-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efa40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
