---
title: 'Range: UsedRange'
description: Возвращает используемый диапазон заданного объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ae8f8bec1eea6f2e13b4c4248d55afbb28cf19d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928068"
---
# <a name="range-usedrange"></a><span data-ttu-id="1a7ed-103">Range: UsedRange</span><span class="sxs-lookup"><span data-stu-id="1a7ed-103">Range: UsedRange</span></span>

> <span data-ttu-id="1a7ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a7ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a7ed-106">Возвращает используемый диапазон заданного объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a7ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a7ed-107">Permissions</span></span>
<span data-ttu-id="1a7ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a7ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a7ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a7ed-110">Permission type</span></span>      | <span data-ttu-id="1a7ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a7ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a7ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a7ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a7ed-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a7ed-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a7ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a7ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a7ed-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a7ed-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a7ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a7ed-116">Application</span></span> | <span data-ttu-id="1a7ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a7ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a7ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="1a7ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a7ed-119">Request headers</span></span>
| <span data-ttu-id="1a7ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1a7ed-120">Name</span></span>       | <span data-ttu-id="1a7ed-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1a7ed-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a7ed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a7ed-122">Authorization</span></span>  | <span data-ttu-id="1a7ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a7ed-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1a7ed-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1a7ed-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7ed-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a7ed-128">Request body</span></span>
<span data-ttu-id="1a7ed-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a7ed-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1a7ed-130">Parameter</span></span>    | <span data-ttu-id="1a7ed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a7ed-131">Type</span></span>   |<span data-ttu-id="1a7ed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a7ed-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a7ed-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="1a7ed-133">valuesOnly</span></span>|<span data-ttu-id="1a7ed-134">boolean</span><span class="sxs-lookup"><span data-stu-id="1a7ed-134">boolean</span></span>|<span data-ttu-id="1a7ed-p105">Необязательный. Учитывает только ячейки со значениями.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="1a7ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a7ed-137">Response</span></span>

<span data-ttu-id="1a7ed-138">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a7ed-139">Пример</span><span class="sxs-lookup"><span data-stu-id="1a7ed-139">Example</span></span>
<span data-ttu-id="1a7ed-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a7ed-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a7ed-141">Request</span></span>
<span data-ttu-id="1a7ed-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="1a7ed-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a7ed-143">Response</span></span>
<span data-ttu-id="1a7ed-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1a7ed-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
