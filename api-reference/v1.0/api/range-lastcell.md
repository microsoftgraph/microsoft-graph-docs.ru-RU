---
title: 'Range: LastCell'
description: .
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5156554c5e094556415a03a7651fd0ffee1bcf33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860279"
---
# <a name="range-lastcell"></a><span data-ttu-id="dee60-103">Range: LastCell</span><span class="sxs-lookup"><span data-stu-id="dee60-103">Range: LastCell</span></span>

<span data-ttu-id="dee60-p101">Возвращает последнюю ячейку в диапазоне. Например, последняя ячейка диапазона B2:D5 — D5.</span><span class="sxs-lookup"><span data-stu-id="dee60-p101">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="dee60-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dee60-106">Permissions</span></span>
<span data-ttu-id="dee60-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee60-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dee60-109">Permission type</span></span>      | <span data-ttu-id="dee60-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dee60-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dee60-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dee60-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dee60-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dee60-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dee60-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dee60-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dee60-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee60-114">Not supported.</span></span>    |
|<span data-ttu-id="dee60-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dee60-115">Application</span></span> | <span data-ttu-id="dee60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee60-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dee60-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dee60-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastCell
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastCell
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastCell

```
## <a name="request-headers"></a><span data-ttu-id="dee60-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dee60-118">Request headers</span></span>
| <span data-ttu-id="dee60-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dee60-119">Name</span></span>       | <span data-ttu-id="dee60-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dee60-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dee60-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dee60-121">Authorization</span></span>  | <span data-ttu-id="dee60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dee60-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dee60-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dee60-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dee60-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dee60-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee60-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dee60-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dee60-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dee60-128">Response</span></span>

<span data-ttu-id="dee60-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dee60-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dee60-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dee60-130">Example</span></span>
<span data-ttu-id="dee60-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dee60-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dee60-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dee60-132">Request</span></span>
<span data-ttu-id="dee60-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dee60-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastCell
```

##### <a name="response"></a><span data-ttu-id="dee60-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dee60-134">Response</span></span>
<span data-ttu-id="dee60-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dee60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastCell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
