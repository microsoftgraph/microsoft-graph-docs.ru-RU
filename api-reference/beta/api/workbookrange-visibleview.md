---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e212315de4917b2322f0ffb6f3ef8630ce57f9da
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979061"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="c9205-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="c9205-104">workbookRange: visibleView</span></span>

<span data-ttu-id="c9205-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9205-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c9205-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9205-106">Permissions</span></span>
<span data-ttu-id="c9205-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9205-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9205-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9205-109">Permission type</span></span>      | <span data-ttu-id="c9205-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9205-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9205-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9205-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9205-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9205-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9205-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9205-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9205-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9205-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c9205-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9205-115">Application</span></span> | <span data-ttu-id="c9205-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9205-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9205-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9205-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="c9205-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9205-118">Request headers</span></span>
| <span data-ttu-id="c9205-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c9205-119">Name</span></span>       | <span data-ttu-id="c9205-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c9205-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9205-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9205-121">Authorization</span></span>  | <span data-ttu-id="c9205-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9205-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9205-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c9205-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c9205-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c9205-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9205-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9205-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c9205-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9205-128">Response</span></span>

<span data-ttu-id="c9205-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9205-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9205-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c9205-130">Example</span></span>
<span data-ttu-id="c9205-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c9205-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9205-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9205-132">Request</span></span>
<span data-ttu-id="c9205-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9205-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9205-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9205-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="c9205-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9205-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9205-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9205-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9205-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9205-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9205-138">Java</span><span class="sxs-lookup"><span data-stu-id="c9205-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c9205-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9205-139">Response</span></span>
<span data-ttu-id="c9205-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9205-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


