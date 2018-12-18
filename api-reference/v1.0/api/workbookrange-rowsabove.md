---
title: 'workbookRange: rowsAbove'
description: Возвращает определенное количество строк над заданным диапазоном.
author: lumine2008
ms.openlocfilehash: d90d46cad9fa68b1270c8877fdad69fea3cedccf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351312"
---
# <a name="workbookrange-rowsabove"></a><span data-ttu-id="617eb-103">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="617eb-103">workbookRange: rowsAbove</span></span>

<span data-ttu-id="617eb-104">Возвращает определенное количество строк над заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="617eb-104">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="617eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="617eb-105">Permissions</span></span>
<span data-ttu-id="617eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="617eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="617eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="617eb-108">Permission type</span></span>      | <span data-ttu-id="617eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="617eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="617eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="617eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="617eb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="617eb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="617eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="617eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="617eb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="617eb-113">Not supported.</span></span>    |
|<span data-ttu-id="617eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="617eb-114">Application</span></span> | <span data-ttu-id="617eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="617eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="617eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="617eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="617eb-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="617eb-117">Function parameters</span></span>

| <span data-ttu-id="617eb-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="617eb-118">Parameter</span></span>    | <span data-ttu-id="617eb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="617eb-119">Type</span></span>   |<span data-ttu-id="617eb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="617eb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="617eb-121">count</span><span class="sxs-lookup"><span data-stu-id="617eb-121">count</span></span>|<span data-ttu-id="617eb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="617eb-122">Int32</span></span>|<span data-ttu-id="617eb-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="617eb-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="617eb-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="617eb-128">Request headers</span></span>
| <span data-ttu-id="617eb-129">Имя</span><span class="sxs-lookup"><span data-stu-id="617eb-129">Name</span></span>       | <span data-ttu-id="617eb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="617eb-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="617eb-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="617eb-131">Authorization</span></span>  | <span data-ttu-id="617eb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="617eb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="617eb-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="617eb-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="617eb-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="617eb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="617eb-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="617eb-137">Request body</span></span>
<span data-ttu-id="617eb-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="617eb-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="617eb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="617eb-139">Response</span></span>
<span data-ttu-id="617eb-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="617eb-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="617eb-141">Пример</span><span class="sxs-lookup"><span data-stu-id="617eb-141">Example</span></span>
<span data-ttu-id="617eb-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="617eb-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="617eb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="617eb-143">Request</span></span>
<span data-ttu-id="617eb-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="617eb-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="617eb-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="617eb-145">Response</span></span>
<span data-ttu-id="617eb-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="617eb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="617eb-149">При вызове без Дополнительно `count` параметра, эта функция возвращает одну строку над диапазоном.</span><span class="sxs-lookup"><span data-stu-id="617eb-149">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="617eb-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="617eb-150">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="617eb-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="617eb-151">Response</span></span>
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