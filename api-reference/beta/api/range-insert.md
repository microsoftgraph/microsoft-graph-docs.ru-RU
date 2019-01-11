---
title: 'Range: insert'
description: Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.
localization_priority: Normal
ms.openlocfilehash: 0e7ab0d729dad4eec7fb455774cfed19bf4f5013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831516"
---
# <a name="range-insert"></a><span data-ttu-id="4da37-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="4da37-104">Range: insert</span></span>

> <span data-ttu-id="4da37-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4da37-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4da37-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da37-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4da37-p103">Вставляет ячейку или диапазон ячеек на лист вместо этого диапазона, а также сдвигает другие ячейки, чтобы освободить место. Возвращает новый объект Range в пустом месте.</span><span class="sxs-lookup"><span data-stu-id="4da37-p103">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="4da37-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4da37-109">Permissions</span></span>
<span data-ttu-id="4da37-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da37-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4da37-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da37-112">Permission type</span></span>      | <span data-ttu-id="4da37-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da37-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4da37-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da37-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4da37-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4da37-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4da37-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da37-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da37-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4da37-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4da37-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4da37-118">Application</span></span> | <span data-ttu-id="4da37-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da37-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4da37-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da37-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="4da37-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4da37-121">Request headers</span></span>
| <span data-ttu-id="4da37-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4da37-122">Name</span></span>       | <span data-ttu-id="4da37-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4da37-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4da37-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4da37-124">Authorization</span></span>  | <span data-ttu-id="4da37-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4da37-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4da37-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4da37-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="4da37-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4da37-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4da37-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4da37-130">Request body</span></span>
<span data-ttu-id="4da37-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4da37-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4da37-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="4da37-132">Parameter</span></span>    | <span data-ttu-id="4da37-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4da37-133">Type</span></span>   |<span data-ttu-id="4da37-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4da37-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4da37-135">shift</span><span class="sxs-lookup"><span data-stu-id="4da37-135">shift</span></span>|<span data-ttu-id="4da37-136">string</span><span class="sxs-lookup"><span data-stu-id="4da37-136">string</span></span>|<span data-ttu-id="4da37-p107">Указывает направление сдвига ячеек.  Возможные значения: `Down`, `Right`.</span><span class="sxs-lookup"><span data-stu-id="4da37-p107">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="4da37-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da37-139">Response</span></span>

<span data-ttu-id="4da37-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4da37-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4da37-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4da37-141">Example</span></span>
<span data-ttu-id="4da37-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4da37-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4da37-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4da37-143">Request</span></span>
<span data-ttu-id="4da37-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4da37-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="4da37-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4da37-145">Response</span></span>
<span data-ttu-id="4da37-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4da37-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
