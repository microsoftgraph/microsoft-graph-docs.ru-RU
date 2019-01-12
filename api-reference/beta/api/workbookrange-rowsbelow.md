---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f924bc2bcb0cd936c84435e0f16babbe58e6a2c4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921467"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="75192-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="75192-103">workbookRange: rowsBelow</span></span>

> <span data-ttu-id="75192-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="75192-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75192-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75192-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75192-106">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="75192-106">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="75192-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75192-107">Permissions</span></span>
<span data-ttu-id="75192-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75192-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75192-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75192-110">Permission type</span></span>      | <span data-ttu-id="75192-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75192-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75192-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75192-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75192-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75192-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75192-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75192-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75192-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75192-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="75192-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75192-116">Application</span></span> | <span data-ttu-id="75192-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75192-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75192-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75192-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="75192-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="75192-119">Function parameters</span></span>

| <span data-ttu-id="75192-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="75192-120">Parameter</span></span>    | <span data-ttu-id="75192-121">Тип</span><span class="sxs-lookup"><span data-stu-id="75192-121">Type</span></span>   |<span data-ttu-id="75192-122">Описание</span><span class="sxs-lookup"><span data-stu-id="75192-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75192-123">count</span><span class="sxs-lookup"><span data-stu-id="75192-123">count</span></span>|<span data-ttu-id="75192-124">Int32</span><span class="sxs-lookup"><span data-stu-id="75192-124">Int32</span></span>|<span data-ttu-id="75192-p103">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="75192-p103">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="75192-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75192-130">Request headers</span></span>
| <span data-ttu-id="75192-131">Имя</span><span class="sxs-lookup"><span data-stu-id="75192-131">Name</span></span>       | <span data-ttu-id="75192-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75192-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="75192-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75192-133">Authorization</span></span>  | <span data-ttu-id="75192-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75192-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75192-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="75192-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="75192-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="75192-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75192-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75192-139">Request body</span></span>
<span data-ttu-id="75192-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75192-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75192-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="75192-141">Response</span></span>

<span data-ttu-id="75192-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75192-142">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75192-143">Пример</span><span class="sxs-lookup"><span data-stu-id="75192-143">Example</span></span>
<span data-ttu-id="75192-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75192-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75192-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="75192-145">Request</span></span>
<span data-ttu-id="75192-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75192-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="75192-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="75192-147">Response</span></span>
<span data-ttu-id="75192-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75192-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
