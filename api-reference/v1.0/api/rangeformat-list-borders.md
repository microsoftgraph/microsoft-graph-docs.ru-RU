---
title: Список границ
description: Получение списка объектов rangeborder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a9bbfcd00391884ae6b9e4c95216d46f1c3fed74
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48461595"
---
# <a name="list-borders"></a><span data-ttu-id="ef4d6-103">Список границ</span><span class="sxs-lookup"><span data-stu-id="ef4d6-103">List borders</span></span>

<span data-ttu-id="ef4d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef4d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef4d6-105">Получение списка объектов rangeborder.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-105">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef4d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef4d6-106">Permissions</span></span>
<span data-ttu-id="ef4d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef4d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef4d6-109">Permission type</span></span>      | <span data-ttu-id="ef4d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef4d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef4d6-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef4d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ef4d6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef4d6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ef4d6-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef4d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef4d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-114">Not supported.</span></span>    |
|<span data-ttu-id="ef4d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef4d6-115">Application</span></span> | <span data-ttu-id="ef4d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef4d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef4d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ef4d6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef4d6-118">Optional query parameters</span></span>
<span data-ttu-id="ef4d6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef4d6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef4d6-120">Request headers</span></span>
| <span data-ttu-id="ef4d6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ef4d6-121">Name</span></span>      |<span data-ttu-id="ef4d6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef4d6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef4d6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef4d6-123">Authorization</span></span>  | <span data-ttu-id="ef4d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef4d6-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ef4d6-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ef4d6-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef4d6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef4d6-129">Request body</span></span>
<span data-ttu-id="ef4d6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef4d6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef4d6-131">Response</span></span>

<span data-ttu-id="ef4d6-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркбукранжебордер](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-132">If successful, this method returns a `200 OK` response code and collection of [WorkbookRangeBorder](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ef4d6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ef4d6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef4d6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef4d6-134">Request</span></span>
<span data-ttu-id="ef4d6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef4d6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4d6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
# <a name="c"></a>[<span data-ttu-id="ef4d6-137">C#</span><span class="sxs-lookup"><span data-stu-id="ef4d6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-borders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef4d6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef4d6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-borders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef4d6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef4d6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-borders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef4d6-140">Java</span><span class="sxs-lookup"><span data-stu-id="ef4d6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-borders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ef4d6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef4d6-141">Response</span></span>
<span data-ttu-id="ef4d6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef4d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
