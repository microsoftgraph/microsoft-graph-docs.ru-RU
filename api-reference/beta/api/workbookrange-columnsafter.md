---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 9bdab549d3dc2511e17df1f838ce5ca146b0485a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890869"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="eeb6e-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="eeb6e-103">workbookRange: columnsAfter</span></span>

> <span data-ttu-id="eeb6e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eeb6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eeb6e-106">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-106">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeb6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb6e-107">Permissions</span></span>
<span data-ttu-id="eeb6e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb6e-110">Permission type</span></span>      | <span data-ttu-id="eeb6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeb6e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeb6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeb6e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eeb6e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb6e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eeb6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeb6e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeb6e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb6e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eeb6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeb6e-116">Application</span></span> | <span data-ttu-id="eeb6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeb6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeb6e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="eeb6e-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="eeb6e-119">Function parameters</span></span>

| <span data-ttu-id="eeb6e-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="eeb6e-120">Parameter</span></span>    | <span data-ttu-id="eeb6e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="eeb6e-121">Type</span></span>   |<span data-ttu-id="eeb6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb6e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb6e-123">count</span><span class="sxs-lookup"><span data-stu-id="eeb6e-123">count</span></span>|<span data-ttu-id="eeb6e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="eeb6e-124">Int32</span></span>|<span data-ttu-id="eeb6e-p103">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="eeb6e-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeb6e-129">Request headers</span></span>
| <span data-ttu-id="eeb6e-130">Имя</span><span class="sxs-lookup"><span data-stu-id="eeb6e-130">Name</span></span>       | <span data-ttu-id="eeb6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb6e-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eeb6e-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeb6e-132">Authorization</span></span>  | <span data-ttu-id="eeb6e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eeb6e-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eeb6e-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="eeb6e-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeb6e-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eeb6e-138">Request body</span></span>
<span data-ttu-id="eeb6e-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeb6e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeb6e-140">Response</span></span>

<span data-ttu-id="eeb6e-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeb6e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="eeb6e-142">Example</span></span>
<span data-ttu-id="eeb6e-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eeb6e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeb6e-144">Request</span></span>
<span data-ttu-id="eeb6e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="eeb6e-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="eeb6e-146">Response</span></span>
<span data-ttu-id="eeb6e-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eeb6e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
