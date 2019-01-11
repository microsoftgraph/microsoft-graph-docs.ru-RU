---
title: 'Range: Row'
description: Возвращает строку из диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 006af432d0ea6e16b38694f37411f576f9fc9ed3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885521"
---
# <a name="range-row"></a><span data-ttu-id="e4b56-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="e4b56-103">Range: Row</span></span>

> <span data-ttu-id="e4b56-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4b56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4b56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4b56-106">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="e4b56-106">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4b56-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b56-107">Permissions</span></span>
<span data-ttu-id="e4b56-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4b56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b56-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4b56-110">Permission type</span></span>      | <span data-ttu-id="e4b56-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4b56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4b56-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4b56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4b56-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4b56-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4b56-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4b56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4b56-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4b56-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e4b56-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4b56-116">Application</span></span> | <span data-ttu-id="e4b56-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b56-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4b56-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4b56-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="e4b56-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4b56-119">Request headers</span></span>
| <span data-ttu-id="e4b56-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e4b56-120">Name</span></span>       | <span data-ttu-id="e4b56-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b56-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4b56-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4b56-122">Authorization</span></span>  | <span data-ttu-id="e4b56-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4b56-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4b56-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e4b56-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e4b56-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e4b56-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4b56-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4b56-128">Request body</span></span>
<span data-ttu-id="e4b56-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e4b56-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e4b56-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4b56-130">Parameter</span></span>    | <span data-ttu-id="e4b56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b56-131">Type</span></span>   |<span data-ttu-id="e4b56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b56-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4b56-133">row</span><span class="sxs-lookup"><span data-stu-id="e4b56-133">row</span></span>|<span data-ttu-id="e4b56-134">number</span><span class="sxs-lookup"><span data-stu-id="e4b56-134">number</span></span>|<span data-ttu-id="e4b56-p105">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="e4b56-p105">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="e4b56-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4b56-137">Response</span></span>

<span data-ttu-id="e4b56-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e4b56-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4b56-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e4b56-139">Example</span></span>
<span data-ttu-id="e4b56-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e4b56-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4b56-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4b56-141">Request</span></span>
<span data-ttu-id="e4b56-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4b56-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_row"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Row
Content-type: application/json
Content-length: 18

{
  "row": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="e4b56-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4b56-143">Response</span></span>
<span data-ttu-id="e4b56-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e4b56-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
