---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f86e9bc3a08d8620f2fe55953456387fc6bd473c
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636928"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="933c7-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="933c7-103">workbookRange: columnsAfter</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="933c7-104">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="933c7-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="933c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="933c7-105">Permissions</span></span>
<span data-ttu-id="933c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="933c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="933c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="933c7-108">Permission type</span></span>      | <span data-ttu-id="933c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="933c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="933c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="933c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="933c7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933c7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="933c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="933c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="933c7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="933c7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="933c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="933c7-114">Application</span></span> | <span data-ttu-id="933c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="933c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="933c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="933c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="933c7-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="933c7-117">Function parameters</span></span>

| <span data-ttu-id="933c7-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="933c7-118">Parameter</span></span>    | <span data-ttu-id="933c7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="933c7-119">Type</span></span>   |<span data-ttu-id="933c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="933c7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="933c7-121">count</span><span class="sxs-lookup"><span data-stu-id="933c7-121">count</span></span>|<span data-ttu-id="933c7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="933c7-122">Int32</span></span>|<span data-ttu-id="933c7-p102">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="933c7-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="933c7-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="933c7-127">Request headers</span></span>
| <span data-ttu-id="933c7-128">Имя</span><span class="sxs-lookup"><span data-stu-id="933c7-128">Name</span></span>       | <span data-ttu-id="933c7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="933c7-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="933c7-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="933c7-130">Authorization</span></span>  | <span data-ttu-id="933c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="933c7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="933c7-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="933c7-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="933c7-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="933c7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="933c7-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="933c7-136">Request body</span></span>
<span data-ttu-id="933c7-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="933c7-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="933c7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="933c7-138">Response</span></span>

<span data-ttu-id="933c7-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="933c7-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="933c7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="933c7-140">Example</span></span>
<span data-ttu-id="933c7-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="933c7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="933c7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="933c7-142">Request</span></span>
<span data-ttu-id="933c7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="933c7-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="933c7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="933c7-144">Response</span></span>
<span data-ttu-id="933c7-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="933c7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="933c7-148">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="933c7-148">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="933c7-149">Языках</span><span class="sxs-lookup"><span data-stu-id="933c7-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrange_columnsafter-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
