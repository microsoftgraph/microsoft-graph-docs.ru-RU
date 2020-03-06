---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f7965f89fb8ce44f8475a86cea1a4e2d45999f2a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508732"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="0eb6b-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="0eb6b-104">workbookRange: visibleView</span></span>

<span data-ttu-id="0eb6b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eb6b-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="0eb6b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb6b-106">Permissions</span></span>
<span data-ttu-id="0eb6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb6b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb6b-109">Permission type</span></span>      | <span data-ttu-id="0eb6b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eb6b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0eb6b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0eb6b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0eb6b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eb6b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-114">Not supported.</span></span>    |
|<span data-ttu-id="0eb6b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eb6b-115">Application</span></span> | <span data-ttu-id="0eb6b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eb6b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="0eb6b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eb6b-118">Request headers</span></span>
| <span data-ttu-id="0eb6b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0eb6b-119">Name</span></span>       | <span data-ttu-id="0eb6b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0eb6b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0eb6b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eb6b-121">Authorization</span></span>  | <span data-ttu-id="0eb6b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0eb6b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0eb6b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0eb6b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb6b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb6b-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="0eb6b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb6b-128">Response</span></span>
<span data-ttu-id="0eb6b-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb6b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0eb6b-130">Example</span></span>
<span data-ttu-id="0eb6b-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0eb6b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb6b-132">Request</span></span>
<span data-ttu-id="0eb6b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0eb6b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eb6b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="0eb6b-135">C#</span><span class="sxs-lookup"><span data-stu-id="0eb6b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0eb6b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0eb6b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0eb6b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0eb6b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0eb6b-138">Java</span><span class="sxs-lookup"><span data-stu-id="0eb6b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0eb6b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb6b-139">Response</span></span>
<span data-ttu-id="0eb6b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eb6b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
