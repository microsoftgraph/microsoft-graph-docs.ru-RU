---
title: Обновление объекта ChartSeries
description: Обновление свойств объекта chartseries.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1772265a833d60cc20fdd55e2b6d1755687bd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823732"
---
# <a name="update-chartseries"></a><span data-ttu-id="b1539-103">Обновление объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b1539-103">Update chartseries</span></span>

<span data-ttu-id="b1539-104">Обновление свойств объекта chartseries.</span><span class="sxs-lookup"><span data-stu-id="b1539-104">Update the properties of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1539-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1539-105">Permissions</span></span>
<span data-ttu-id="b1539-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1539-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1539-108">Permission type</span></span>      | <span data-ttu-id="b1539-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1539-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1539-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1539-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1539-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1539-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b1539-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1539-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1539-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1539-113">Not supported.</span></span>    |
|<span data-ttu-id="b1539-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1539-114">Application</span></span> | <span data-ttu-id="b1539-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1539-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1539-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1539-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b1539-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1539-117">Optional request headers</span></span>
| <span data-ttu-id="b1539-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1539-118">Name</span></span>       | <span data-ttu-id="b1539-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b1539-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b1539-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1539-120">Authorization</span></span>  | <span data-ttu-id="b1539-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1539-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1539-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b1539-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b1539-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b1539-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1539-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1539-126">Request body</span></span>
<span data-ttu-id="b1539-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b1539-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b1539-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1539-130">Property</span></span>     | <span data-ttu-id="b1539-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1539-131">Type</span></span>   |<span data-ttu-id="b1539-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1539-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1539-133">name</span><span class="sxs-lookup"><span data-stu-id="b1539-133">name</span></span>|<span data-ttu-id="b1539-134">строка</span><span class="sxs-lookup"><span data-stu-id="b1539-134">string</span></span>|<span data-ttu-id="b1539-135">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="b1539-135">Represents the name of a series in a chart.</span></span>|

## <a name="response"></a><span data-ttu-id="b1539-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1539-136">Response</span></span>

<span data-ttu-id="b1539-137">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookChartSeries](../resources/chartseries.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1539-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1539-138">Пример</span><span class="sxs-lookup"><span data-stu-id="b1539-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1539-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1539-139">Request</span></span>
<span data-ttu-id="b1539-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1539-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartseries"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="b1539-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1539-141">Response</span></span>
<span data-ttu-id="b1539-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b1539-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartseries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
