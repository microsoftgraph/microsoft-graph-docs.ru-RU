---
title: Обновление объекта RangeBorder
description: Обновление свойств объекта rangeborder.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a85bd70b3e8448dd460c2d572ab319142c17bd52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818293"
---
# <a name="update-rangeborder"></a><span data-ttu-id="dd95b-103">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="dd95b-103">Update rangeborder</span></span>

<span data-ttu-id="dd95b-104">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="dd95b-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd95b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd95b-105">Permissions</span></span>
<span data-ttu-id="dd95b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd95b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd95b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd95b-108">Permission type</span></span>      | <span data-ttu-id="dd95b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd95b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd95b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd95b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd95b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd95b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd95b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd95b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd95b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd95b-113">Not supported.</span></span>    |
|<span data-ttu-id="dd95b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd95b-114">Application</span></span> | <span data-ttu-id="dd95b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd95b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd95b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd95b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dd95b-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd95b-117">Optional request headers</span></span>
| <span data-ttu-id="dd95b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dd95b-118">Name</span></span>       | <span data-ttu-id="dd95b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dd95b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dd95b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd95b-120">Authorization</span></span>  | <span data-ttu-id="dd95b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd95b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd95b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd95b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd95b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd95b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd95b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd95b-126">Request body</span></span>
<span data-ttu-id="dd95b-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dd95b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd95b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd95b-130">Property</span></span>     | <span data-ttu-id="dd95b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd95b-131">Type</span></span>   |<span data-ttu-id="dd95b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd95b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd95b-133">color</span><span class="sxs-lookup"><span data-stu-id="dd95b-133">color</span></span>|<span data-ttu-id="dd95b-134">строка</span><span class="sxs-lookup"><span data-stu-id="dd95b-134">string</span></span>|<span data-ttu-id="dd95b-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="dd95b-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="dd95b-136">style</span><span class="sxs-lookup"><span data-stu-id="dd95b-136">style</span></span>|<span data-ttu-id="dd95b-137">строка</span><span class="sxs-lookup"><span data-stu-id="dd95b-137">string</span></span>|<span data-ttu-id="dd95b-138">Одна из констант линии, определяющее тип линии границы.</span><span class="sxs-lookup"><span data-stu-id="dd95b-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="dd95b-139">Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="dd95b-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="dd95b-140">weight</span><span class="sxs-lookup"><span data-stu-id="dd95b-140">weight</span></span>|<span data-ttu-id="dd95b-141">string</span><span class="sxs-lookup"><span data-stu-id="dd95b-141">string</span></span>|<span data-ttu-id="dd95b-142">Задает Вес границы вокруг диапазона.</span><span class="sxs-lookup"><span data-stu-id="dd95b-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="dd95b-143">Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="dd95b-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="dd95b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd95b-144">Response</span></span>

<span data-ttu-id="dd95b-145">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленный объект [WorkbookRangeBorder](../resources/rangeborder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dd95b-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd95b-146">Пример</span><span class="sxs-lookup"><span data-stu-id="dd95b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd95b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd95b-147">Request</span></span>
<span data-ttu-id="dd95b-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd95b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="dd95b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd95b-149">Response</span></span>
<span data-ttu-id="dd95b-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dd95b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
