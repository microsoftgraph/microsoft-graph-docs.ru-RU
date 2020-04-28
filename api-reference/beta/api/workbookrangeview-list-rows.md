---
title: Получение списка строк rangeView
description: Получение списка, который включает в себя объекты видимых ячеек в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 48196e700e081d466d4fbd8f2bed2b8f2cbd7f74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451324"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="1f838-103">Получение списка строк rangeView</span><span class="sxs-lookup"><span data-stu-id="1f838-103">List rangeView rows</span></span>

<span data-ttu-id="1f838-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f838-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f838-105">Получение списка, который включает в себя объекты видимых ячеек в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="1f838-105">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f838-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f838-106">Permissions</span></span>
<span data-ttu-id="1f838-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f838-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f838-109">Permission type</span></span>      | <span data-ttu-id="1f838-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f838-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f838-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f838-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f838-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f838-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f838-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f838-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f838-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f838-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f838-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f838-115">Application</span></span> | <span data-ttu-id="1f838-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f838-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f838-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f838-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f838-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f838-118">Optional query parameters</span></span>
<span data-ttu-id="1f838-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f838-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f838-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f838-120">Request headers</span></span>
| <span data-ttu-id="1f838-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1f838-121">Name</span></span>      |<span data-ttu-id="1f838-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1f838-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f838-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f838-123">Authorization</span></span>  | <span data-ttu-id="1f838-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f838-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f838-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f838-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f838-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1f838-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f838-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f838-129">Request body</span></span>
<span data-ttu-id="1f838-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f838-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f838-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f838-131">Response</span></span>

<span data-ttu-id="1f838-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f838-132">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f838-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f838-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f838-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f838-134">Request</span></span>
<span data-ttu-id="1f838-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f838-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f838-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f838-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows 
```
# <a name="c"></a>[<span data-ttu-id="1f838-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f838-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f838-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f838-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f838-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f838-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f838-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f838-140">Response</span></span>
<span data-ttu-id="1f838-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f838-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
