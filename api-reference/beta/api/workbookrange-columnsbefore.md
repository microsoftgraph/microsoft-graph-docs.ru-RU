---
title: 'workbookRange: columnsBefore'
description: Возвращает определенное количество столбцов слева от заданного диапазона.
author: lumine2008
ms.openlocfilehash: b53b998655b079c0d875efb50263a0492373a696
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344711"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="51aa8-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="51aa8-103">workbookRange: columnsBefore</span></span>

> <span data-ttu-id="51aa8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51aa8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51aa8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51aa8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51aa8-106">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="51aa8-106">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="51aa8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51aa8-107">Permissions</span></span>
<span data-ttu-id="51aa8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51aa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51aa8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51aa8-110">Permission type</span></span>      | <span data-ttu-id="51aa8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51aa8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51aa8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51aa8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51aa8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51aa8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="51aa8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51aa8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51aa8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51aa8-115">Not supported.</span></span>    |
|<span data-ttu-id="51aa8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51aa8-116">Application</span></span> | <span data-ttu-id="51aa8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51aa8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51aa8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51aa8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="51aa8-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="51aa8-119">Function parameters</span></span>

| <span data-ttu-id="51aa8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="51aa8-120">Parameter</span></span>    | <span data-ttu-id="51aa8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="51aa8-121">Type</span></span>   |<span data-ttu-id="51aa8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="51aa8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51aa8-123">count</span><span class="sxs-lookup"><span data-stu-id="51aa8-123">count</span></span>|<span data-ttu-id="51aa8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="51aa8-124">Int32</span></span>|<span data-ttu-id="51aa8-p103">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="51aa8-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="51aa8-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51aa8-129">Request headers</span></span>
| <span data-ttu-id="51aa8-130">Имя</span><span class="sxs-lookup"><span data-stu-id="51aa8-130">Name</span></span>       | <span data-ttu-id="51aa8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51aa8-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51aa8-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51aa8-132">Authorization</span></span>  | <span data-ttu-id="51aa8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51aa8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51aa8-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="51aa8-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="51aa8-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="51aa8-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51aa8-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51aa8-138">Request body</span></span>
<span data-ttu-id="51aa8-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51aa8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51aa8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="51aa8-140">Response</span></span>
<span data-ttu-id="51aa8-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51aa8-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51aa8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="51aa8-142">Example</span></span>
<span data-ttu-id="51aa8-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="51aa8-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51aa8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="51aa8-144">Request</span></span>
<span data-ttu-id="51aa8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51aa8-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="51aa8-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="51aa8-146">Response</span></span>
<span data-ttu-id="51aa8-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51aa8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
