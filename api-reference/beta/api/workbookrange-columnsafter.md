---
title: 'workbookRange: columnsAfter'
description: Возвращает определенное количество столбцов справа от заданного диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3623cfb0b4dc487a1e15e6b1c29726433700b04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522016"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="4e86b-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="4e86b-103">workbookRange: columnsAfter</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e86b-104">Возвращает определенное количество столбцов справа от заданного диапазона.</span><span class="sxs-lookup"><span data-stu-id="4e86b-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e86b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e86b-105">Permissions</span></span>
<span data-ttu-id="4e86b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e86b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e86b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e86b-108">Permission type</span></span>      | <span data-ttu-id="4e86b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e86b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e86b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e86b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e86b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e86b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e86b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e86b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e86b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e86b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e86b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e86b-114">Application</span></span> | <span data-ttu-id="4e86b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e86b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e86b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e86b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="4e86b-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4e86b-117">Function parameters</span></span>

| <span data-ttu-id="4e86b-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e86b-118">Parameter</span></span>    | <span data-ttu-id="4e86b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4e86b-119">Type</span></span>   |<span data-ttu-id="4e86b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e86b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e86b-121">count</span><span class="sxs-lookup"><span data-stu-id="4e86b-121">count</span></span>|<span data-ttu-id="4e86b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4e86b-122">Int32</span></span>|<span data-ttu-id="4e86b-p102">Количество столбцов, которые нужно включить в результирующий диапазон. Чтобы создать диапазон за пределами текущего диапазона, используйте положительное число. Вы также можете указать отрицательное число, чтобы создать диапазон в рамках текущего диапазона. По умолчанию используется значение 1.</span><span class="sxs-lookup"><span data-stu-id="4e86b-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4e86b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e86b-127">Request headers</span></span>
| <span data-ttu-id="4e86b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="4e86b-128">Name</span></span>       | <span data-ttu-id="4e86b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4e86b-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e86b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e86b-130">Authorization</span></span>  | <span data-ttu-id="4e86b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e86b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e86b-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e86b-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e86b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e86b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e86b-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e86b-136">Request body</span></span>
<span data-ttu-id="4e86b-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e86b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e86b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e86b-138">Response</span></span>

<span data-ttu-id="4e86b-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRange](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e86b-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e86b-140">Пример</span><span class="sxs-lookup"><span data-stu-id="4e86b-140">Example</span></span>
<span data-ttu-id="4e86b-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4e86b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e86b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e86b-142">Request</span></span>
<span data-ttu-id="4e86b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e86b-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="4e86b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e86b-144">Response</span></span>
<span data-ttu-id="4e86b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4e86b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/workbookrange-columnsafter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
