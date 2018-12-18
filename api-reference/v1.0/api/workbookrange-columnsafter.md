---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
ms.openlocfilehash: b80657c6afb7709049a1e0ccaa3c3b232f5501c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304237"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="1e4da-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="1e4da-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="1e4da-104">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="1e4da-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e4da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4da-105">Permissions</span></span>
<span data-ttu-id="1e4da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4da-108">Permission type</span></span>      | <span data-ttu-id="1e4da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e4da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e4da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e4da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e4da-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e4da-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e4da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e4da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e4da-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e4da-113">Not supported.</span></span>    |
|<span data-ttu-id="1e4da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e4da-114">Application</span></span> | <span data-ttu-id="1e4da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e4da-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e4da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e4da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="1e4da-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="1e4da-117">Function parameters</span></span>

| <span data-ttu-id="1e4da-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="1e4da-118">Parameter</span></span>    | <span data-ttu-id="1e4da-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1e4da-119">Type</span></span>   |<span data-ttu-id="1e4da-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1e4da-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e4da-121">count</span><span class="sxs-lookup"><span data-stu-id="1e4da-121">count</span></span>|<span data-ttu-id="1e4da-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4da-122">Int32</span></span>|<span data-ttu-id="1e4da-123">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="1e4da-123">Optional.</span></span> <span data-ttu-id="1e4da-124">Число столбцов для включения в результирующий диапазон.</span><span class="sxs-lookup"><span data-stu-id="1e4da-124">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="1e4da-125">В общем случае используйте положительное число для создания диапазона за пределами текущего диапазона.</span><span class="sxs-lookup"><span data-stu-id="1e4da-125">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="1e4da-126">Отрицательное значение можно также использовать для создания диапазона в текущем диапазоне.</span><span class="sxs-lookup"><span data-stu-id="1e4da-126">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="1e4da-127">Значение по умолчанию — 1</span><span class="sxs-lookup"><span data-stu-id="1e4da-127">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1e4da-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e4da-128">Request headers</span></span>
| <span data-ttu-id="1e4da-129">Имя</span><span class="sxs-lookup"><span data-stu-id="1e4da-129">Name</span></span>       | <span data-ttu-id="1e4da-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1e4da-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e4da-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e4da-131">Authorization</span></span>  | <span data-ttu-id="1e4da-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e4da-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e4da-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1e4da-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e4da-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1e4da-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e4da-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e4da-137">Request body</span></span>
<span data-ttu-id="1e4da-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e4da-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e4da-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e4da-139">Response</span></span>
<span data-ttu-id="1e4da-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1e4da-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4da-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1e4da-141">Example</span></span>
<span data-ttu-id="1e4da-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1e4da-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e4da-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e4da-143">Request</span></span>
<span data-ttu-id="1e4da-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e4da-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="1e4da-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e4da-145">Response</span></span>
<span data-ttu-id="1e4da-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1e4da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
