---
title: 'workbookRange: resizedRange'
description: Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e9e332a3ec35dcb5177021ae4057f8f61cf1434c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995911"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="0d2b5-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="0d2b5-103">workbookRange: resizedRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d2b5-104">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d2b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2b5-105">Permissions</span></span>
<span data-ttu-id="0d2b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d2b5-108">Permission type</span></span>      | <span data-ttu-id="0d2b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d2b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d2b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2b5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d2b5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0d2b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d2b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2b5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d2b5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0d2b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d2b5-114">Application</span></span> | <span data-ttu-id="0d2b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d2b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="0d2b5-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0d2b5-117">Function parameters</span></span>

| <span data-ttu-id="0d2b5-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d2b5-118">Parameter</span></span>    | <span data-ttu-id="0d2b5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0d2b5-119">Type</span></span>   |<span data-ttu-id="0d2b5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2b5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d2b5-121">deltarows</span><span class="sxs-lookup"><span data-stu-id="0d2b5-121">deltarows</span></span>|<span data-ttu-id="0d2b5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0d2b5-122">Int32</span></span>|<span data-ttu-id="0d2b5-p102">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="0d2b5-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="0d2b5-125">deltaColumns</span></span>|<span data-ttu-id="0d2b5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0d2b5-126">Int32</span></span>|<span data-ttu-id="0d2b5-p103">Количество столбцов, добавляемых в правый нижний угол, относительно текущего диапазона. Используйте положительное число, чтобы расширить диапазон или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p103">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="0d2b5-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d2b5-129">Request headers</span></span>
| <span data-ttu-id="0d2b5-130">Имя</span><span class="sxs-lookup"><span data-stu-id="0d2b5-130">Name</span></span>       | <span data-ttu-id="0d2b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d2b5-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d2b5-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d2b5-132">Authorization</span></span>  | <span data-ttu-id="0d2b5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d2b5-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0d2b5-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="0d2b5-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d2b5-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d2b5-138">Request body</span></span>
<span data-ttu-id="0d2b5-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d2b5-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d2b5-140">Response</span></span>

<span data-ttu-id="0d2b5-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d2b5-142">Пример</span><span class="sxs-lookup"><span data-stu-id="0d2b5-142">Example</span></span>
<span data-ttu-id="0d2b5-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0d2b5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d2b5-144">Request</span></span>
<span data-ttu-id="0d2b5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="0d2b5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d2b5-146">Response</span></span>
<span data-ttu-id="0d2b5-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d2b5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
