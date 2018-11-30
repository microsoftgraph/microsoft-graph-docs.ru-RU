---
title: Обновление объекта ChartLineFormat
description: Обновление свойств объекта chartlineformat.
ms.openlocfilehash: 543177af0288c476c31d27b618a187a3a0f9a1a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026449"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="bc5e5-103">Обновление объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="bc5e5-103">Update chartlineformat</span></span>

<span data-ttu-id="bc5e5-104">Обновление свойств объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc5e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc5e5-105">Permissions</span></span>
<span data-ttu-id="bc5e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc5e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc5e5-108">Permission type</span></span>      | <span data-ttu-id="bc5e5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc5e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc5e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc5e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc5e5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc5e5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc5e5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc5e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5e5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-113">Not supported.</span></span>    |
|<span data-ttu-id="bc5e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc5e5-114">Application</span></span> | <span data-ttu-id="bc5e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc5e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc5e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="bc5e5-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc5e5-117">Optional request headers</span></span>
| <span data-ttu-id="bc5e5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bc5e5-118">Name</span></span>       | <span data-ttu-id="bc5e5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bc5e5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bc5e5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc5e5-120">Authorization</span></span>  | <span data-ttu-id="bc5e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc5e5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc5e5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc5e5-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc5e5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc5e5-126">Request body</span></span>
<span data-ttu-id="bc5e5-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc5e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc5e5-130">Property</span></span>     | <span data-ttu-id="bc5e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc5e5-131">Type</span></span>   |<span data-ttu-id="bc5e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc5e5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc5e5-133">color</span><span class="sxs-lookup"><span data-stu-id="bc5e5-133">color</span></span>|<span data-ttu-id="bc5e5-134">строка</span><span class="sxs-lookup"><span data-stu-id="bc5e5-134">string</span></span>|<span data-ttu-id="bc5e5-135">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="bc5e5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc5e5-136">Response</span></span>

<span data-ttu-id="bc5e5-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartLineFormat](../resources/chartlineformat.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc5e5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="bc5e5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc5e5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc5e5-139">Request</span></span>
<span data-ttu-id="bc5e5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc5e5-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="bc5e5-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc5e5-141">Response</span></span>
<span data-ttu-id="bc5e5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bc5e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->