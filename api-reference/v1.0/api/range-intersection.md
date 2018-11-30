---
title: 'Range: Intersection'
description: Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.
ms.openlocfilehash: e2480630435a8fdf7195af1d174e6141e5f068c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024895"
---
# <a name="range-intersection"></a><span data-ttu-id="9ec2e-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="9ec2e-103">Range: Intersection</span></span>

<span data-ttu-id="9ec2e-104">Возвращает объект диапазона, представляющий собой прямоугольное пересечение заданных диапазонов.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-104">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ec2e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec2e-105">Permissions</span></span>
<span data-ttu-id="9ec2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec2e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec2e-108">Permission type</span></span>      | <span data-ttu-id="9ec2e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ec2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ec2e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ec2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ec2e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ec2e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9ec2e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ec2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec2e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-113">Not supported.</span></span>    |
|<span data-ttu-id="9ec2e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ec2e-114">Application</span></span> | <span data-ttu-id="9ec2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec2e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ec2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/intersection

```
## <a name="request-headers"></a><span data-ttu-id="9ec2e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ec2e-117">Request headers</span></span>
| <span data-ttu-id="9ec2e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9ec2e-118">Name</span></span>       | <span data-ttu-id="9ec2e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9ec2e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ec2e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ec2e-120">Authorization</span></span>  | <span data-ttu-id="9ec2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ec2e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9ec2e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9ec2e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec2e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ec2e-126">Request body</span></span>
<span data-ttu-id="9ec2e-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9ec2e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ec2e-128">Parameter</span></span>    | <span data-ttu-id="9ec2e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9ec2e-129">Type</span></span>   |<span data-ttu-id="9ec2e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9ec2e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ec2e-131">anotherRange</span><span class="sxs-lookup"><span data-stu-id="9ec2e-131">anotherRange</span></span>|<span data-ttu-id="9ec2e-132">string</span><span class="sxs-lookup"><span data-stu-id="9ec2e-132">string</span></span>|<span data-ttu-id="9ec2e-133">Объект или адрес диапазона, который будет использоваться для определения пересечения диапазонов.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-133">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="9ec2e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ec2e-134">Response</span></span>

<span data-ttu-id="9ec2e-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec2e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9ec2e-136">Example</span></span>
<span data-ttu-id="9ec2e-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ec2e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ec2e-138">Request</span></span>
<span data-ttu-id="9ec2e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ec2e-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="9ec2e-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ec2e-140">Response</span></span>
<span data-ttu-id="9ec2e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9ec2e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->