---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
ms.openlocfilehash: cab5fd162e8df1fda7f8376b87580e7a882f2a7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026275"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="7504c-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="7504c-103">workbookRange: rowsBelow</span></span>

<span data-ttu-id="7504c-104">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="7504c-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7504c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7504c-105">Permissions</span></span>
<span data-ttu-id="7504c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7504c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7504c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7504c-108">Permission type</span></span>      | <span data-ttu-id="7504c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7504c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7504c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7504c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7504c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7504c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7504c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7504c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7504c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7504c-113">Not supported.</span></span>    |
|<span data-ttu-id="7504c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7504c-114">Application</span></span> | <span data-ttu-id="7504c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7504c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7504c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7504c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="7504c-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7504c-117">Function parameters</span></span>

| <span data-ttu-id="7504c-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="7504c-118">Parameter</span></span>    | <span data-ttu-id="7504c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7504c-119">Type</span></span>   |<span data-ttu-id="7504c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7504c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7504c-121">count</span><span class="sxs-lookup"><span data-stu-id="7504c-121">count</span></span>|<span data-ttu-id="7504c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7504c-122">Int32</span></span>| <span data-ttu-id="7504c-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="7504c-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7504c-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7504c-128">Request headers</span></span>
| <span data-ttu-id="7504c-129">Имя</span><span class="sxs-lookup"><span data-stu-id="7504c-129">Name</span></span>       | <span data-ttu-id="7504c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7504c-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7504c-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7504c-131">Authorization</span></span>  | <span data-ttu-id="7504c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7504c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7504c-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7504c-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="7504c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7504c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7504c-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7504c-137">Request body</span></span>
<span data-ttu-id="7504c-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7504c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7504c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7504c-139">Response</span></span>
<span data-ttu-id="7504c-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7504c-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7504c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7504c-141">Example</span></span>
<span data-ttu-id="7504c-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7504c-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7504c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7504c-143">Request</span></span>
<span data-ttu-id="7504c-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7504c-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="7504c-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="7504c-145">Response</span></span>
<span data-ttu-id="7504c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7504c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="7504c-149">При вызове без `count` параметр, по умолчанию эта функция на одну строку.</span><span class="sxs-lookup"><span data-stu-id="7504c-149">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="7504c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7504c-150">Request</span></span>
<span data-ttu-id="7504c-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7504c-151">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="7504c-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="7504c-152">Response</span></span>
<span data-ttu-id="7504c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7504c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
