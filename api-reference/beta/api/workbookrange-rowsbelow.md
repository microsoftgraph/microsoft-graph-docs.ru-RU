---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f3f070cbbbed4dc4018f56a95b98240bd9ffc599
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339722"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="46a60-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="46a60-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46a60-104">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="46a60-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="46a60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46a60-105">Permissions</span></span>
<span data-ttu-id="46a60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46a60-108">Permission type</span></span>      | <span data-ttu-id="46a60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46a60-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46a60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46a60-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46a60-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a60-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46a60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46a60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46a60-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46a60-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="46a60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46a60-114">Application</span></span> | <span data-ttu-id="46a60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a60-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46a60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46a60-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="46a60-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="46a60-117">Function parameters</span></span>

| <span data-ttu-id="46a60-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="46a60-118">Parameter</span></span>    | <span data-ttu-id="46a60-119">Тип</span><span class="sxs-lookup"><span data-stu-id="46a60-119">Type</span></span>   |<span data-ttu-id="46a60-120">Описание</span><span class="sxs-lookup"><span data-stu-id="46a60-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46a60-121">count</span><span class="sxs-lookup"><span data-stu-id="46a60-121">count</span></span>|<span data-ttu-id="46a60-122">Int32</span><span class="sxs-lookup"><span data-stu-id="46a60-122">Int32</span></span>|<span data-ttu-id="46a60-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="46a60-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="46a60-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46a60-128">Request headers</span></span>
| <span data-ttu-id="46a60-129">Имя</span><span class="sxs-lookup"><span data-stu-id="46a60-129">Name</span></span>       | <span data-ttu-id="46a60-130">Описание</span><span class="sxs-lookup"><span data-stu-id="46a60-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="46a60-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46a60-131">Authorization</span></span>  | <span data-ttu-id="46a60-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46a60-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46a60-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46a60-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="46a60-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="46a60-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a60-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46a60-137">Request body</span></span>
<span data-ttu-id="46a60-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46a60-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a60-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="46a60-139">Response</span></span>

<span data-ttu-id="46a60-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/workbookrange.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46a60-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46a60-141">Пример</span><span class="sxs-lookup"><span data-stu-id="46a60-141">Example</span></span>
<span data-ttu-id="46a60-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="46a60-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="46a60-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="46a60-143">Request</span></span>
<span data-ttu-id="46a60-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46a60-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="46a60-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a60-145">Response</span></span>
<span data-ttu-id="46a60-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46a60-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
