---
title: 'workbookRange: resizedRange'
description: Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.
ms.openlocfilehash: 167aef7a1d7c975298b80d9e27aad7043b276b35
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025271"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="937fa-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="937fa-103">workbookRange: resizedRange</span></span>
<span data-ttu-id="937fa-104">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="937fa-104">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="937fa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="937fa-105">Permissions</span></span>
<span data-ttu-id="937fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937fa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937fa-108">Permission type</span></span>      | <span data-ttu-id="937fa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="937fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937fa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="937fa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="937fa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="937fa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937fa-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937fa-113">Not supported.</span></span>    |
|<span data-ttu-id="937fa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="937fa-114">Application</span></span> | <span data-ttu-id="937fa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="937fa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="937fa-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="937fa-117">Function parameters</span></span>

| <span data-ttu-id="937fa-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="937fa-118">Parameter</span></span>    | <span data-ttu-id="937fa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="937fa-119">Type</span></span>   |<span data-ttu-id="937fa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="937fa-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="937fa-121">deltaRows</span><span class="sxs-lookup"><span data-stu-id="937fa-121">deltaRows</span></span>|<span data-ttu-id="937fa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="937fa-122">Int32</span></span>|<span data-ttu-id="937fa-p102">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="937fa-p102">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="937fa-125">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="937fa-125">deltaColumns</span></span>|<span data-ttu-id="937fa-126">Int32</span><span class="sxs-lookup"><span data-stu-id="937fa-126">Int32</span></span>|<span data-ttu-id="937fa-127">Число столбцов, с помощью которого разверните нижний правый угол относительно текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="937fa-127">The number of columns by which to expand the bottom-right corner, relative to the current range.</span></span> <span data-ttu-id="937fa-128">Используйте положительное число, чтобы расширить диапазон или отрицательное значение, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="937fa-128">Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="937fa-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="937fa-129">Request headers</span></span>
| <span data-ttu-id="937fa-130">Имя</span><span class="sxs-lookup"><span data-stu-id="937fa-130">Name</span></span>       | <span data-ttu-id="937fa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="937fa-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="937fa-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="937fa-132">Authorization</span></span>  | <span data-ttu-id="937fa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="937fa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="937fa-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="937fa-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="937fa-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="937fa-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="937fa-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="937fa-138">Request body</span></span>
<span data-ttu-id="937fa-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="937fa-139">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="937fa-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="937fa-140">Response</span></span>
<span data-ttu-id="937fa-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="937fa-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937fa-142">Пример</span><span class="sxs-lookup"><span data-stu-id="937fa-142">Example</span></span>
<span data-ttu-id="937fa-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="937fa-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="937fa-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="937fa-144">Request</span></span>
<span data-ttu-id="937fa-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="937fa-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="937fa-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="937fa-146">Response</span></span>
<span data-ttu-id="937fa-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="937fa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
