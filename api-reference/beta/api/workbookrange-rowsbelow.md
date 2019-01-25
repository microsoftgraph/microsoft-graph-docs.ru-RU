---
title: 'workbookRange: rowsBelow'
description: Возвращает определенное количество строк под заданным диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 42d53ce3aa9d26c7c499b19af3d5330259786520
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529476"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="d7bd5-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="d7bd5-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7bd5-104">Возвращает определенное количество строк под заданным диапазоном.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7bd5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7bd5-105">Permissions</span></span>
<span data-ttu-id="d7bd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7bd5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7bd5-108">Permission type</span></span>      | <span data-ttu-id="d7bd5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7bd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7bd5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7bd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7bd5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7bd5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7bd5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7bd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7bd5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7bd5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7bd5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7bd5-114">Application</span></span> | <span data-ttu-id="d7bd5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7bd5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7bd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="d7bd5-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d7bd5-117">Function parameters</span></span>

| <span data-ttu-id="d7bd5-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="d7bd5-118">Parameter</span></span>    | <span data-ttu-id="d7bd5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d7bd5-119">Type</span></span>   |<span data-ttu-id="d7bd5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d7bd5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7bd5-121">count</span><span class="sxs-lookup"><span data-stu-id="d7bd5-121">count</span></span>|<span data-ttu-id="d7bd5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d7bd5-122">Int32</span></span>|<span data-ttu-id="d7bd5-p102">Необязательный. Количество строк, включаемых в полученный диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d7bd5-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7bd5-128">Request headers</span></span>
| <span data-ttu-id="d7bd5-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d7bd5-129">Name</span></span>       | <span data-ttu-id="d7bd5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d7bd5-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7bd5-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7bd5-131">Authorization</span></span>  | <span data-ttu-id="d7bd5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7bd5-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7bd5-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7bd5-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7bd5-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7bd5-137">Request body</span></span>
<span data-ttu-id="d7bd5-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7bd5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7bd5-139">Response</span></span>

<span data-ttu-id="d7bd5-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7bd5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d7bd5-141">Example</span></span>
<span data-ttu-id="d7bd5-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7bd5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7bd5-143">Request</span></span>
<span data-ttu-id="d7bd5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7bd5-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="d7bd5-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7bd5-145">Response</span></span>
<span data-ttu-id="d7bd5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d7bd5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
