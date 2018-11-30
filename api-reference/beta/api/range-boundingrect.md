---
title: 'Range: BoundingRect'
description: .
ms.openlocfilehash: 25a313fca1fe73c0717777b4dabc4c9b6eb9372f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074802"
---
# <a name="range-boundingrect"></a><span data-ttu-id="ab465-103">Range: BoundingRect</span><span class="sxs-lookup"><span data-stu-id="ab465-103">Range: BoundingRect</span></span>

> <span data-ttu-id="ab465-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab465-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab465-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab465-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab465-p102">Возвращает наименьший объект диапазона, включающий в себя заданные диапазоны. Например, GetBoundingRect для "B2:C5" и "D10:E15" — "B2:E16".</span><span class="sxs-lookup"><span data-stu-id="ab465-p102">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="ab465-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab465-108">Permissions</span></span>
<span data-ttu-id="ab465-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab465-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab465-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab465-111">Permission type</span></span>      | <span data-ttu-id="ab465-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab465-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab465-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab465-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ab465-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab465-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab465-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab465-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab465-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab465-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab465-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab465-117">Application</span></span> | <span data-ttu-id="ab465-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab465-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab465-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab465-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="ab465-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab465-120">Request headers</span></span>
| <span data-ttu-id="ab465-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ab465-121">Name</span></span>       | <span data-ttu-id="ab465-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ab465-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab465-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab465-123">Authorization</span></span>  | <span data-ttu-id="ab465-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab465-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab465-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ab465-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ab465-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ab465-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab465-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab465-129">Request body</span></span>
<span data-ttu-id="ab465-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ab465-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ab465-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ab465-131">Parameter</span></span>    | <span data-ttu-id="ab465-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ab465-132">Type</span></span>   |<span data-ttu-id="ab465-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ab465-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab465-134">anotherRange</span><span class="sxs-lookup"><span data-stu-id="ab465-134">anotherRange</span></span>|<span data-ttu-id="ab465-135">string</span><span class="sxs-lookup"><span data-stu-id="ab465-135">string</span></span>|<span data-ttu-id="ab465-136">Объект, адрес или имя диапазона.</span><span class="sxs-lookup"><span data-stu-id="ab465-136">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="ab465-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab465-137">Response</span></span>

<span data-ttu-id="ab465-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab465-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab465-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ab465-139">Example</span></span>
<span data-ttu-id="ab465-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ab465-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab465-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab465-141">Request</span></span>
<span data-ttu-id="ab465-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab465-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="ab465-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab465-143">Response</span></span>
<span data-ttu-id="ab465-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ab465-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->