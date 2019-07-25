---
title: Получение объекта TableSort
description: Получение свойств и связей объекта tablesort.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ef030993c42f2154f04cf6020785749385d5baf0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868447"
---
# <a name="get-tablesort"></a><span data-ttu-id="922fb-103">Получение объекта TableSort</span><span class="sxs-lookup"><span data-stu-id="922fb-103">Get TableSort</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="922fb-104">Получение свойств и связей объекта tablesort.</span><span class="sxs-lookup"><span data-stu-id="922fb-104">Retrieve the properties and relationships of tablesort object.</span></span>
## <a name="permissions"></a><span data-ttu-id="922fb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="922fb-105">Permissions</span></span>
<span data-ttu-id="922fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="922fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="922fb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="922fb-108">Permission type</span></span>      | <span data-ttu-id="922fb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="922fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="922fb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="922fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="922fb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="922fb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="922fb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="922fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="922fb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="922fb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="922fb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="922fb-114">Application</span></span> | <span data-ttu-id="922fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="922fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="922fb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="922fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort
```
## <a name="optional-query-parameters"></a><span data-ttu-id="922fb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="922fb-117">Optional query parameters</span></span>
<span data-ttu-id="922fb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="922fb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="922fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="922fb-119">Request headers</span></span>
| <span data-ttu-id="922fb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="922fb-120">Name</span></span>      |<span data-ttu-id="922fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="922fb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="922fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="922fb-122">Authorization</span></span>  | <span data-ttu-id="922fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="922fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="922fb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="922fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="922fb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="922fb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="922fb-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="922fb-128">Request body</span></span>
<span data-ttu-id="922fb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="922fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="922fb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="922fb-130">Response</span></span>

<span data-ttu-id="922fb-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбуктаблесорт](../resources/workbooktablesort.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="922fb-131">If successful, this method returns a `200 OK` response code and [workbookTableSort](../resources/workbooktablesort.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="922fb-132">Пример</span><span class="sxs-lookup"><span data-stu-id="922fb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="922fb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="922fb-133">Request</span></span>
<span data-ttu-id="922fb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="922fb-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="922fb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="922fb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tablesort"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="922fb-136">C#</span><span class="sxs-lookup"><span data-stu-id="922fb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tablesort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="922fb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="922fb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tablesort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="922fb-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="922fb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tablesort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="922fb-139">Java</span><span class="sxs-lookup"><span data-stu-id="922fb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tablesort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="922fb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="922fb-140">Response</span></span>
<span data-ttu-id="922fb-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="922fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableSort"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "matchCase": true,
  "method": "method-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get TableSort",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
