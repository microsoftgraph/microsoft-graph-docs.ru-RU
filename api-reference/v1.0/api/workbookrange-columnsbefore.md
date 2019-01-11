---
title: 'workbookRange: columnsBefore'
description: Возвращает определенное количество столбцов слева от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2d8316ff9a13dbe4770aef10139c1075aca01241
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867853"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="7ba23-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="7ba23-103">workbookRange: columnsBefore</span></span>

<span data-ttu-id="7ba23-104">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="7ba23-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ba23-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ba23-105">Permissions</span></span>
<span data-ttu-id="7ba23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ba23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ba23-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ba23-108">Permission type</span></span>      | <span data-ttu-id="7ba23-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ba23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ba23-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ba23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ba23-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ba23-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ba23-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ba23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ba23-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba23-113">Not supported.</span></span>    |
|<span data-ttu-id="7ba23-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ba23-114">Application</span></span> | <span data-ttu-id="7ba23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ba23-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ba23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="7ba23-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7ba23-117">Function parameters</span></span>

| <span data-ttu-id="7ba23-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ba23-118">Parameter</span></span>    | <span data-ttu-id="7ba23-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7ba23-119">Type</span></span>   |<span data-ttu-id="7ba23-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba23-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ba23-121">count</span><span class="sxs-lookup"><span data-stu-id="7ba23-121">count</span></span>|<span data-ttu-id="7ba23-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7ba23-122">Int32</span></span>|<span data-ttu-id="7ba23-p102">Необязательный. Количество столбцов, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="7ba23-p102">Optional. The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7ba23-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ba23-128">Request headers</span></span>
| <span data-ttu-id="7ba23-129">Имя</span><span class="sxs-lookup"><span data-stu-id="7ba23-129">Name</span></span>       | <span data-ttu-id="7ba23-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba23-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ba23-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ba23-131">Authorization</span></span>  | <span data-ttu-id="7ba23-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ba23-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ba23-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7ba23-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ba23-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7ba23-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba23-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ba23-137">Request body</span></span>
<span data-ttu-id="7ba23-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ba23-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ba23-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ba23-139">Response</span></span>
<span data-ttu-id="7ba23-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ba23-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba23-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7ba23-141">Example</span></span>
<span data-ttu-id="7ba23-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7ba23-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ba23-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ba23-143">Request</span></span>
<span data-ttu-id="7ba23-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ba23-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsbefore",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="7ba23-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ba23-145">Response</span></span>
<span data-ttu-id="7ba23-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ba23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
