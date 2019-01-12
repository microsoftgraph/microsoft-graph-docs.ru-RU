---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eca10cb28689f7e4f850e1dbd3c7fb4fbd932649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972462"
---
# <a name="range-lastrow"></a><span data-ttu-id="7296b-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="7296b-103">Range: LastRow</span></span>

<span data-ttu-id="7296b-p101">Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="7296b-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="7296b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7296b-106">Permissions</span></span>
<span data-ttu-id="7296b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7296b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7296b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7296b-109">Permission type</span></span>      | <span data-ttu-id="7296b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7296b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7296b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7296b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7296b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7296b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7296b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7296b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7296b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7296b-114">Not supported.</span></span>    |
|<span data-ttu-id="7296b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7296b-115">Application</span></span> | <span data-ttu-id="7296b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7296b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7296b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7296b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastRow

```
## <a name="request-headers"></a><span data-ttu-id="7296b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7296b-118">Request headers</span></span>
| <span data-ttu-id="7296b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7296b-119">Name</span></span>       | <span data-ttu-id="7296b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7296b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7296b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7296b-121">Authorization</span></span>  | <span data-ttu-id="7296b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7296b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7296b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7296b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7296b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7296b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7296b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7296b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7296b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7296b-128">Response</span></span>

<span data-ttu-id="7296b-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7296b-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7296b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7296b-130">Example</span></span>
<span data-ttu-id="7296b-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7296b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7296b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7296b-132">Request</span></span>
<span data-ttu-id="7296b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7296b-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastRow
```

##### <a name="response"></a><span data-ttu-id="7296b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7296b-134">Response</span></span>
<span data-ttu-id="7296b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7296b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
