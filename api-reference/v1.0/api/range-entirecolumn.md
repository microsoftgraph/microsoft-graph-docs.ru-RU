---
title: 'Range: EntireColumn'
description: Возвращает объект, представляющий весь столбец диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 99de7bfff2008702722ba07a84b04c02d50b3e69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851718"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="87cc1-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="87cc1-103">Range: EntireColumn</span></span>

<span data-ttu-id="87cc1-104">Возвращает объект, представляющий весь столбец диапазона.</span><span class="sxs-lookup"><span data-stu-id="87cc1-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="87cc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87cc1-105">Permissions</span></span>
<span data-ttu-id="87cc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87cc1-108">Permission type</span></span>      | <span data-ttu-id="87cc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87cc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87cc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87cc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87cc1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cc1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="87cc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87cc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87cc1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87cc1-113">Not supported.</span></span>    |
|<span data-ttu-id="87cc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87cc1-114">Application</span></span> | <span data-ttu-id="87cc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87cc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87cc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87cc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="87cc1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87cc1-117">Request headers</span></span>
| <span data-ttu-id="87cc1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="87cc1-118">Name</span></span>       | <span data-ttu-id="87cc1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="87cc1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87cc1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87cc1-120">Authorization</span></span>  | <span data-ttu-id="87cc1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87cc1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87cc1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="87cc1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="87cc1-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="87cc1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87cc1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87cc1-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="87cc1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="87cc1-127">Response</span></span>

<span data-ttu-id="87cc1-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="87cc1-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87cc1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="87cc1-129">Example</span></span>
<span data-ttu-id="87cc1-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="87cc1-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87cc1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="87cc1-131">Request</span></span>
<span data-ttu-id="87cc1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87cc1-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```

##### <a name="response"></a><span data-ttu-id="87cc1-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="87cc1-133">Response</span></span>
<span data-ttu-id="87cc1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87cc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
