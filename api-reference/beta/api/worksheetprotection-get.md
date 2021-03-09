---
title: Get workbookWorksheetProtection
description: Извлечение свойств и связей объекта workbookworksheetprotection.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5741a9ed6e24519f704d0c2df13d62945e36d13b
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578147"
---
# <a name="get-workbookworksheetprotection"></a><span data-ttu-id="214bf-103">Get workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="214bf-103">Get workbookWorksheetProtection</span></span>

<span data-ttu-id="214bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="214bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="214bf-105">Извлечение свойств и связей объекта workbookWorksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="214bf-105">Retrieve the properties and relationships of workbookWorksheetProtection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="214bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="214bf-106">Permissions</span></span>
<span data-ttu-id="214bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="214bf-109">Permission type</span></span>      | <span data-ttu-id="214bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="214bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="214bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="214bf-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214bf-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="214bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214bf-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214bf-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="214bf-115">Application</span></span> | <span data-ttu-id="214bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214bf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="214bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="214bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/protection
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="214bf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="214bf-118">Optional query parameters</span></span>
<span data-ttu-id="214bf-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="214bf-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="214bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="214bf-120">Request headers</span></span>
| <span data-ttu-id="214bf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="214bf-121">Name</span></span>      |<span data-ttu-id="214bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="214bf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="214bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="214bf-123">Authorization</span></span>  | <span data-ttu-id="214bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="214bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="214bf-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="214bf-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="214bf-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="214bf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="214bf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="214bf-129">Request body</span></span>
<span data-ttu-id="214bf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="214bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214bf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="214bf-131">Response</span></span>

<span data-ttu-id="214bf-132">В случае успеха этот метод возвращает код отклика и объект `200 OK` [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="214bf-132">If successful, this method returns a `200 OK` response code and [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="214bf-133">Пример</span><span class="sxs-lookup"><span data-stu-id="214bf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="214bf-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="214bf-134">Request</span></span>
<span data-ttu-id="214bf-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="214bf-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="214bf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="214bf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection
```
# <a name="c"></a>[<span data-ttu-id="214bf-137">C#</span><span class="sxs-lookup"><span data-stu-id="214bf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookworksheetprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="214bf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="214bf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookworksheetprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="214bf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="214bf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookworksheetprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="214bf-140">Java</span><span class="sxs-lookup"><span data-stu-id="214bf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookworksheetprotection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="214bf-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="214bf-141">Response</span></span>
<span data-ttu-id="214bf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="214bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 23

{
  "protected": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookWorksheetProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
