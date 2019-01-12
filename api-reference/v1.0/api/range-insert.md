---
title: 'Range: insert'
description: Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: aa59abfd2b60454a73472fc5283d3c7212ee48ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929048"
---
# <a name="range-insert"></a><span data-ttu-id="fcd7e-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="fcd7e-104">Range: insert</span></span>

<span data-ttu-id="fcd7e-p102">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcd7e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd7e-107">Permissions</span></span>
<span data-ttu-id="fcd7e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcd7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcd7e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcd7e-110">Permission type</span></span>      | <span data-ttu-id="fcd7e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcd7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcd7e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcd7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fcd7e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcd7e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fcd7e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcd7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcd7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-115">Not supported.</span></span>    |
|<span data-ttu-id="fcd7e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcd7e-116">Application</span></span> | <span data-ttu-id="fcd7e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcd7e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcd7e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="fcd7e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcd7e-119">Request headers</span></span>
| <span data-ttu-id="fcd7e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fcd7e-120">Name</span></span>       | <span data-ttu-id="fcd7e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fcd7e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fcd7e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcd7e-122">Authorization</span></span>  | <span data-ttu-id="fcd7e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fcd7e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fcd7e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fcd7e-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcd7e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcd7e-128">Request body</span></span>
<span data-ttu-id="fcd7e-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fcd7e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="fcd7e-130">Parameter</span></span>    | <span data-ttu-id="fcd7e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcd7e-131">Type</span></span>   |<span data-ttu-id="fcd7e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcd7e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcd7e-133">shift</span><span class="sxs-lookup"><span data-stu-id="fcd7e-133">shift</span></span>|<span data-ttu-id="fcd7e-134">string</span><span class="sxs-lookup"><span data-stu-id="fcd7e-134">string</span></span>|<span data-ttu-id="fcd7e-135">Указывает, каким способом сдвига ячеек.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="fcd7e-136">Возможные значения: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="fcd7e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcd7e-137">Response</span></span>

<span data-ttu-id="fcd7e-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcd7e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="fcd7e-139">Example</span></span>
<span data-ttu-id="fcd7e-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fcd7e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcd7e-141">Request</span></span>
<span data-ttu-id="fcd7e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="fcd7e-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcd7e-143">Response</span></span>
<span data-ttu-id="fcd7e-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcd7e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
