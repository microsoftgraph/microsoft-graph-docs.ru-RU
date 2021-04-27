---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d7d6eb63c60728eb7969d99bf6e1eb5e9eed596a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053309"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="892f6-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="892f6-104">workbookRange: visibleView</span></span>

<span data-ttu-id="892f6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="892f6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="892f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="892f6-106">Permissions</span></span>
<span data-ttu-id="892f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="892f6-109">Permission type</span></span>      | <span data-ttu-id="892f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="892f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="892f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="892f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="892f6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892f6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="892f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892f6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892f6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="892f6-115">Application</span></span> | <span data-ttu-id="892f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="892f6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="892f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="892f6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="892f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="892f6-118">Request headers</span></span>
| <span data-ttu-id="892f6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="892f6-119">Name</span></span>       | <span data-ttu-id="892f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="892f6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="892f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="892f6-121">Authorization</span></span>  | <span data-ttu-id="892f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="892f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="892f6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="892f6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="892f6-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="892f6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="892f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="892f6-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="892f6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="892f6-128">Response</span></span>

<span data-ttu-id="892f6-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="892f6-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892f6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="892f6-130">Example</span></span>
<span data-ttu-id="892f6-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="892f6-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="892f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="892f6-132">Request</span></span>
<span data-ttu-id="892f6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="892f6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="892f6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="892f6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="892f6-135">C#</span><span class="sxs-lookup"><span data-stu-id="892f6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="892f6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="892f6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="892f6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="892f6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="892f6-138">Java</span><span class="sxs-lookup"><span data-stu-id="892f6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="892f6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="892f6-139">Response</span></span>
<span data-ttu-id="892f6-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="892f6-140">Here is an example of the response.</span></span> <span data-ttu-id="892f6-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="892f6-141">Note: The response object shown here might be shortened for readability.</span></span>
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


