---
title: Список NamedItemCollection
description: Получение списка объектов nameditem.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e9e5709d9e2d47ac2c8bf06984df145f9507a39c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983771"
---
# <a name="list-nameditemcollection"></a><span data-ttu-id="6c985-103">Список NamedItemCollection</span><span class="sxs-lookup"><span data-stu-id="6c985-103">List NamedItemCollection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c985-104">Получение списка объектов nameditem.</span><span class="sxs-lookup"><span data-stu-id="6c985-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c985-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c985-105">Permissions</span></span>
<span data-ttu-id="6c985-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c985-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c985-108">Permission type</span></span>      | <span data-ttu-id="6c985-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c985-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c985-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c985-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c985-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c985-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c985-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c985-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c985-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c985-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6c985-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c985-114">Application</span></span> | <span data-ttu-id="6c985-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c985-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c985-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c985-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c985-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c985-117">Optional query parameters</span></span>
<span data-ttu-id="6c985-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c985-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c985-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c985-119">Request headers</span></span>
| <span data-ttu-id="6c985-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6c985-120">Name</span></span>      |<span data-ttu-id="6c985-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6c985-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c985-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c985-122">Authorization</span></span>  | <span data-ttu-id="6c985-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c985-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c985-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6c985-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6c985-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6c985-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c985-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c985-128">Request body</span></span>
<span data-ttu-id="6c985-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c985-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c985-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c985-130">Response</span></span>

<span data-ttu-id="6c985-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукнамедитем](../resources/workbooknameditem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c985-131">If successful, this method returns a `200 OK` response code and collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c985-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6c985-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c985-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c985-133">Request</span></span>
<span data-ttu-id="6c985-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c985-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6c985-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c985-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_nameditemcollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6c985-136">C#</span><span class="sxs-lookup"><span data-stu-id="6c985-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-nameditemcollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c985-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c985-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-nameditemcollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6c985-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6c985-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-nameditemcollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6c985-139">Java</span><span class="sxs-lookup"><span data-stu-id="6c985-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-nameditemcollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6c985-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c985-140">Response</span></span>
<span data-ttu-id="6c985-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c985-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List NamedItemCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
