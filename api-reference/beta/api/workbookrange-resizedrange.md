---
title: 'workbookRange: resizedRange'
description: Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.
ms.openlocfilehash: cd2851e1b4f65162fca6e617878851b2cc8e910b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077133"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="f1348-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="f1348-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="f1348-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1348-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1348-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1348-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1348-106">Возвращает объект диапазона, подобный текущему объекту диапазона, но увеличенный (или уменьшенный) на некоторое количество строк и столбцов в правом нижнем углу.</span><span class="sxs-lookup"><span data-stu-id="f1348-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1348-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1348-107">Permissions</span></span>
<span data-ttu-id="f1348-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1348-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1348-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1348-110">Permission type</span></span>      | <span data-ttu-id="f1348-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1348-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1348-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1348-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f1348-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1348-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1348-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1348-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1348-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1348-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1348-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1348-116">Application</span></span> | <span data-ttu-id="f1348-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1348-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1348-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1348-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="f1348-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="f1348-119">Function parameters</span></span>

| <span data-ttu-id="f1348-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="f1348-120">Parameter</span></span>    | <span data-ttu-id="f1348-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f1348-121">Type</span></span>   |<span data-ttu-id="f1348-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f1348-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1348-123">deltarows</span><span class="sxs-lookup"><span data-stu-id="f1348-123">deltarows</span></span>|<span data-ttu-id="f1348-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f1348-124">Int32</span></span>|<span data-ttu-id="f1348-p103">Количество строк, добавляемых в правый нижний угол текущего диапазона. Используйте положительное число, чтобы расширить диапазон, или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="f1348-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="f1348-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="f1348-127">deltaColumns</span></span>|<span data-ttu-id="f1348-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f1348-128">Int32</span></span>|<span data-ttu-id="f1348-p104">Количество столбцов, добавляемых в правый нижний угол, относительно текущего диапазона. Используйте положительное число, чтобы расширить диапазон или отрицательное число, чтобы уменьшить его.</span><span class="sxs-lookup"><span data-stu-id="f1348-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f1348-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1348-131">Request headers</span></span>
| <span data-ttu-id="f1348-132">Имя</span><span class="sxs-lookup"><span data-stu-id="f1348-132">Name</span></span>       | <span data-ttu-id="f1348-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f1348-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1348-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1348-134">Authorization</span></span>  | <span data-ttu-id="f1348-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1348-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1348-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1348-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1348-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f1348-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1348-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1348-140">Request body</span></span>
<span data-ttu-id="f1348-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1348-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1348-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1348-142">Response</span></span>

<span data-ttu-id="f1348-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1348-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1348-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f1348-144">Example</span></span>
<span data-ttu-id="f1348-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f1348-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1348-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1348-146">Request</span></span>
<span data-ttu-id="f1348-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1348-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="f1348-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1348-148">Response</span></span>
<span data-ttu-id="f1348-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f1348-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
