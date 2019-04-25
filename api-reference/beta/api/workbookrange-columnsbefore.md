---
title: 'workbookRange: columnsBefore'
description: Возвращает определенное количество столбцов слева от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 677ee0d20031a9973644eec63e0a87e9c47440b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536092"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="fc3b6-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="fc3b6-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc3b6-104">Возвращает определенное количество столбцов слева от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc3b6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc3b6-105">Permissions</span></span>
<span data-ttu-id="fc3b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc3b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc3b6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc3b6-108">Permission type</span></span>      | <span data-ttu-id="fc3b6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc3b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc3b6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc3b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc3b6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc3b6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fc3b6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc3b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc3b6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-113">Not supported.</span></span>    |
|<span data-ttu-id="fc3b6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc3b6-114">Application</span></span> | <span data-ttu-id="fc3b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc3b6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc3b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="fc3b6-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fc3b6-117">Function parameters</span></span>

| <span data-ttu-id="fc3b6-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc3b6-118">Parameter</span></span>    | <span data-ttu-id="fc3b6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fc3b6-119">Type</span></span>   |<span data-ttu-id="fc3b6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc3b6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc3b6-121">count</span><span class="sxs-lookup"><span data-stu-id="fc3b6-121">count</span></span>|<span data-ttu-id="fc3b6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="fc3b6-122">Int32</span></span>|<span data-ttu-id="fc3b6-p102">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете использовать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fc3b6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc3b6-127">Request headers</span></span>
| <span data-ttu-id="fc3b6-128">Имя</span><span class="sxs-lookup"><span data-stu-id="fc3b6-128">Name</span></span>       | <span data-ttu-id="fc3b6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="fc3b6-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc3b6-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc3b6-130">Authorization</span></span>  | <span data-ttu-id="fc3b6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc3b6-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fc3b6-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="fc3b6-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc3b6-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc3b6-136">Request body</span></span>
<span data-ttu-id="fc3b6-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc3b6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc3b6-138">Response</span></span>
<span data-ttu-id="fc3b6-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc3b6-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fc3b6-140">Example</span></span>
<span data-ttu-id="fc3b6-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc3b6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc3b6-142">Request</span></span>
<span data-ttu-id="fc3b6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="fc3b6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc3b6-144">Response</span></span>
<span data-ttu-id="fc3b6-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc3b6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/workbookrange-columnsbefore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
