---
title: 'Range: Row'
description: Возвращает строку из диапазона.
author: lumine2008
ms.openlocfilehash: d758af607fa80314abe6c3f90e611eb87ac62914
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315031"
---
# <a name="range-row"></a><span data-ttu-id="f3121-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="f3121-103">Range: Row</span></span>

<span data-ttu-id="f3121-104">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="f3121-104">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3121-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3121-105">Permissions</span></span>
<span data-ttu-id="f3121-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3121-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3121-108">Permission type</span></span>      | <span data-ttu-id="f3121-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3121-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3121-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3121-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3121-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3121-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f3121-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3121-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3121-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3121-113">Not supported.</span></span>    |
|<span data-ttu-id="f3121-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3121-114">Application</span></span> | <span data-ttu-id="f3121-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3121-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3121-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3121-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/row
POST /workbook/worksheets/{id|name}/range(address='<address>')/row
POST /workbook/tables/{id|name}/columns/{id|name}/range/row

```
## <a name="request-headers"></a><span data-ttu-id="f3121-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3121-117">Request headers</span></span>
| <span data-ttu-id="f3121-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f3121-118">Name</span></span>       | <span data-ttu-id="f3121-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f3121-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3121-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3121-120">Authorization</span></span>  | <span data-ttu-id="f3121-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3121-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f3121-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f3121-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f3121-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3121-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3121-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3121-126">Request body</span></span>
<span data-ttu-id="f3121-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f3121-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f3121-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="f3121-128">Parameter</span></span>    | <span data-ttu-id="f3121-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f3121-129">Type</span></span>   |<span data-ttu-id="f3121-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f3121-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3121-131">row</span><span class="sxs-lookup"><span data-stu-id="f3121-131">row</span></span>|<span data-ttu-id="f3121-132">Int32</span><span class="sxs-lookup"><span data-stu-id="f3121-132">Int32</span></span>|<span data-ttu-id="f3121-p104">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="f3121-p104">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f3121-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3121-135">Response</span></span>

<span data-ttu-id="f3121-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3121-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3121-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f3121-137">Example</span></span>
<span data-ttu-id="f3121-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f3121-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f3121-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3121-139">Request</span></span>
<span data-ttu-id="f3121-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3121-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_row",
  "idempotent": true,
  "@type": "requestBodyResourceFor.range_row"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/row
Content-type: application/json
Content-length: 18

{
  "row": 2
}
```

##### <a name="response"></a><span data-ttu-id="f3121-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3121-141">Response</span></span>
<span data-ttu-id="f3121-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f3121-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Row",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->