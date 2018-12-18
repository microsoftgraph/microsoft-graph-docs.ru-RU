---
title: 'TableColumnCollection: add'
description: Добавляет новый столбец в таблицу.
author: lumine2008
ms.openlocfilehash: a0897dc4eff387d14643b0a067ef92ad79755614
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350024"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="c5d90-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="c5d90-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="c5d90-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5d90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5d90-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5d90-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5d90-106">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="c5d90-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5d90-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5d90-107">Permissions</span></span>
<span data-ttu-id="c5d90-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5d90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d90-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5d90-110">Permission type</span></span>      | <span data-ttu-id="c5d90-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5d90-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d90-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5d90-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5d90-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5d90-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5d90-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5d90-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5d90-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5d90-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c5d90-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5d90-116">Application</span></span> | <span data-ttu-id="c5d90-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5d90-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5d90-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5d90-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="c5d90-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5d90-119">Request headers</span></span>
| <span data-ttu-id="c5d90-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c5d90-120">Name</span></span>       | <span data-ttu-id="c5d90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c5d90-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5d90-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5d90-122">Authorization</span></span>  | <span data-ttu-id="c5d90-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5d90-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5d90-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c5d90-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c5d90-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c5d90-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d90-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5d90-128">Request body</span></span>
<span data-ttu-id="c5d90-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5d90-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5d90-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5d90-130">Parameter</span></span>    | <span data-ttu-id="c5d90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5d90-131">Type</span></span>   |<span data-ttu-id="c5d90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5d90-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5d90-133">index</span><span class="sxs-lookup"><span data-stu-id="c5d90-133">index</span></span>|<span data-ttu-id="c5d90-134">number</span><span class="sxs-lookup"><span data-stu-id="c5d90-134">number</span></span>|<span data-ttu-id="c5d90-p105">Определяет относительную позицию нового столбца. Предыдущий столбец на этой позиции сдвигается вправо. Значение индекса должно быть равно или меньше значения индекса последнего столбца, чтобы его невозможно было использовать для добавления столбца в конце таблицы. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="c5d90-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="c5d90-139">values</span><span class="sxs-lookup"><span data-stu-id="c5d90-139">values</span></span>|<span data-ttu-id="c5d90-140">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="c5d90-140">(boolean or string or number)</span></span>|<span data-ttu-id="c5d90-p106">Необязательный параметр. Двухмерный массив неформатированных значений столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="c5d90-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="c5d90-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5d90-143">Response</span></span>

<span data-ttu-id="c5d90-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5d90-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5d90-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c5d90-145">Example</span></span>
<span data-ttu-id="c5d90-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c5d90-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5d90-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5d90-147">Request</span></span>
<span data-ttu-id="c5d90-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5d90-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="c5d90-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5d90-149">Response</span></span>
<span data-ttu-id="c5d90-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5d90-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->