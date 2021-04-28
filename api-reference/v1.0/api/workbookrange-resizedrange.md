---
title: 'workbookRange: resizedRange'
description: Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 89dc3cf7635bb858cf1a818059e21a31c09da77a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055661"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="81bcc-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="81bcc-103">workbookRange: resizedRange</span></span>

<span data-ttu-id="81bcc-104">Пространство имен: microsoft.graph получает объект диапазона, похожий на текущий объект диапазона, но с его нижним правым углом, расширенным (или законтрактованым) рядом строк и столбцов.</span><span class="sxs-lookup"><span data-stu-id="81bcc-104">Namespace: microsoft.graph Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="81bcc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81bcc-105">Permissions</span></span>
<span data-ttu-id="81bcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81bcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81bcc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81bcc-108">Permission type</span></span>      | <span data-ttu-id="81bcc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81bcc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81bcc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81bcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81bcc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81bcc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81bcc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81bcc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81bcc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bcc-113">Not supported.</span></span>    |
|<span data-ttu-id="81bcc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81bcc-114">Application</span></span> | <span data-ttu-id="81bcc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bcc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81bcc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81bcc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="81bcc-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="81bcc-117">Function parameters</span></span>

| <span data-ttu-id="81bcc-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="81bcc-118">Parameter</span></span>    | <span data-ttu-id="81bcc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="81bcc-119">Type</span></span>   |<span data-ttu-id="81bcc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="81bcc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81bcc-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="81bcc-121">deltaRows</span></span>|<span data-ttu-id="81bcc-122">Int32</span><span class="sxs-lookup"><span data-stu-id="81bcc-122">Int32</span></span>|<span data-ttu-id="81bcc-p102">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="81bcc-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="81bcc-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="81bcc-125">deltaColumns</span></span>|<span data-ttu-id="81bcc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="81bcc-126">Int32</span></span>|<span data-ttu-id="81bcc-127">Количество столбцов, с помощью которых можно расширить нижний правый угол по отношению к текущему диапазону.</span><span class="sxs-lookup"><span data-stu-id="81bcc-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="81bcc-128">Используйте положительное число, чтобы расширить диапазон или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="81bcc-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="81bcc-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81bcc-129">Request headers</span></span>
| <span data-ttu-id="81bcc-130">Имя</span><span class="sxs-lookup"><span data-stu-id="81bcc-130">Name</span></span>       | <span data-ttu-id="81bcc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81bcc-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81bcc-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81bcc-132">Authorization</span></span>  | <span data-ttu-id="81bcc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81bcc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81bcc-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="81bcc-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="81bcc-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="81bcc-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81bcc-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81bcc-138">Request body</span></span>
<span data-ttu-id="81bcc-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81bcc-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="81bcc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="81bcc-140">Response</span></span>
<span data-ttu-id="81bcc-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81bcc-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81bcc-142">Пример</span><span class="sxs-lookup"><span data-stu-id="81bcc-142">Example</span></span>
<span data-ttu-id="81bcc-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="81bcc-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81bcc-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="81bcc-144">Request</span></span>
<span data-ttu-id="81bcc-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81bcc-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="81bcc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="81bcc-146">Response</span></span>
<span data-ttu-id="81bcc-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81bcc-147">Here is an example of the response.</span></span> <span data-ttu-id="81bcc-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81bcc-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

