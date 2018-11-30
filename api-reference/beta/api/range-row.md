---
title: 'Range: Row'
description: Возвращает строку из диапазона.
ms.openlocfilehash: d27d604444760d31f4abed9f1c3b9ae958a34aee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080378"
---
# <a name="range-row"></a><span data-ttu-id="ecb9f-103">Range: Row</span><span class="sxs-lookup"><span data-stu-id="ecb9f-103">Range: Row</span></span>

> <span data-ttu-id="ecb9f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecb9f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecb9f-106">Возвращает строку из диапазона.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-106">Gets a row contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="ecb9f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb9f-107">Permissions</span></span>
<span data-ttu-id="ecb9f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb9f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb9f-110">Permission type</span></span>      | <span data-ttu-id="ecb9f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecb9f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb9f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecb9f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb9f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecb9f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ecb9f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecb9f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb9f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ecb9f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ecb9f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecb9f-116">Application</span></span> | <span data-ttu-id="ecb9f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecb9f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecb9f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/Row
POST /workbook/worksheets/{id|name}/range(address='<address>')/Row
POST /workbook/tables/{id|name}/columns/{id|name}/range/Row

```
## <a name="request-headers"></a><span data-ttu-id="ecb9f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecb9f-119">Request headers</span></span>
| <span data-ttu-id="ecb9f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ecb9f-120">Name</span></span>       | <span data-ttu-id="ecb9f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb9f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ecb9f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecb9f-122">Authorization</span></span>  | <span data-ttu-id="ecb9f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ecb9f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ecb9f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ecb9f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb9f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecb9f-128">Request body</span></span>
<span data-ttu-id="ecb9f-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ecb9f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ecb9f-130">Parameter</span></span>    | <span data-ttu-id="ecb9f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ecb9f-131">Type</span></span>   |<span data-ttu-id="ecb9f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb9f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb9f-133">row</span><span class="sxs-lookup"><span data-stu-id="ecb9f-133">row</span></span>|<span data-ttu-id="ecb9f-134">number</span><span class="sxs-lookup"><span data-stu-id="ecb9f-134">number</span></span>|<span data-ttu-id="ecb9f-p105">Номер строки диапазона, который требуется извлечь. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-p105">Row number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="ecb9f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb9f-137">Response</span></span>

<span data-ttu-id="ecb9f-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb9f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ecb9f-139">Example</span></span>
<span data-ttu-id="ecb9f-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ecb9f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecb9f-141">Request</span></span>
<span data-ttu-id="ecb9f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecb9f-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ecb9f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecb9f-143">Response</span></span>
<span data-ttu-id="ecb9f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ecb9f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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