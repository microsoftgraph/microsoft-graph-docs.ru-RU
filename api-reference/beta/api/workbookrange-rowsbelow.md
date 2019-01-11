---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4ca004f60756b4c6408b40a7a5602456284cafb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845152"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="e7535-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="e7535-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="e7535-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7535-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7535-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7535-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7535-106">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="e7535-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7535-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7535-107">Permissions</span></span>
<span data-ttu-id="e7535-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7535-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7535-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7535-110">Permission type</span></span>      | <span data-ttu-id="e7535-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7535-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7535-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7535-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7535-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7535-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7535-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7535-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7535-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7535-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7535-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7535-116">Application</span></span> | <span data-ttu-id="e7535-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7535-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7535-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7535-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="e7535-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="e7535-119">Function parameters</span></span>

| <span data-ttu-id="e7535-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7535-120">Parameter</span></span>    | <span data-ttu-id="e7535-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e7535-121">Type</span></span>   |<span data-ttu-id="e7535-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e7535-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7535-123">count</span><span class="sxs-lookup"><span data-stu-id="e7535-123">count</span></span>|<span data-ttu-id="e7535-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e7535-124">Int32</span></span>|<span data-ttu-id="e7535-p103">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="e7535-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e7535-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7535-130">Request headers</span></span>
| <span data-ttu-id="e7535-131">Имя</span><span class="sxs-lookup"><span data-stu-id="e7535-131">Name</span></span>       | <span data-ttu-id="e7535-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7535-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7535-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7535-133">Authorization</span></span>  | <span data-ttu-id="e7535-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7535-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7535-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7535-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7535-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e7535-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7535-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7535-139">Request body</span></span>
<span data-ttu-id="e7535-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7535-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7535-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7535-141">Response</span></span>

<span data-ttu-id="e7535-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7535-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7535-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e7535-143">Example</span></span>
<span data-ttu-id="e7535-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e7535-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e7535-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7535-145">Request</span></span>
<span data-ttu-id="e7535-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7535-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="e7535-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7535-147">Response</span></span>
<span data-ttu-id="e7535-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7535-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
