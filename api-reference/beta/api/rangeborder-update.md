---
title: Обновление объекта RangeBorder
description: Обновление свойств объекта rangeborder.
author: lumine2008
ms.openlocfilehash: 560848adf8e2ff663c3b3a223786c24ba3b53c42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349303"
---
# <a name="update-rangeborder"></a><span data-ttu-id="1c1d7-103">Обновление объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="1c1d7-103">Update rangeborder</span></span>

> <span data-ttu-id="1c1d7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c1d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c1d7-106">Обновление свойств объекта rangeborder.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c1d7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c1d7-107">Permissions</span></span>
<span data-ttu-id="1c1d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c1d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c1d7-110">Permission type</span></span>      | <span data-ttu-id="1c1d7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c1d7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c1d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c1d7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c1d7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c1d7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c1d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c1d7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c1d7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c1d7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c1d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c1d7-116">Application</span></span> | <span data-ttu-id="1c1d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c1d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c1d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="1c1d7-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c1d7-119">Optional request headers</span></span>
| <span data-ttu-id="1c1d7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1c1d7-120">Name</span></span>       | <span data-ttu-id="1c1d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1c1d7-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1c1d7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c1d7-122">Authorization</span></span>  | <span data-ttu-id="1c1d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c1d7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c1d7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c1d7-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c1d7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c1d7-128">Request body</span></span>
<span data-ttu-id="1c1d7-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c1d7-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c1d7-132">Property</span></span>     | <span data-ttu-id="1c1d7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1c1d7-133">Type</span></span>   |<span data-ttu-id="1c1d7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1c1d7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c1d7-135">color</span><span class="sxs-lookup"><span data-stu-id="1c1d7-135">color</span></span>|<span data-ttu-id="1c1d7-136">строка</span><span class="sxs-lookup"><span data-stu-id="1c1d7-136">string</span></span>|<span data-ttu-id="1c1d7-137">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="1c1d7-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="1c1d7-138">style</span><span class="sxs-lookup"><span data-stu-id="1c1d7-138">style</span></span>|<span data-ttu-id="1c1d7-139">строка</span><span class="sxs-lookup"><span data-stu-id="1c1d7-139">string</span></span>|<span data-ttu-id="1c1d7-p106">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="1c1d7-142">weight</span><span class="sxs-lookup"><span data-stu-id="1c1d7-142">weight</span></span>|<span data-ttu-id="1c1d7-143">string</span><span class="sxs-lookup"><span data-stu-id="1c1d7-143">string</span></span>|<span data-ttu-id="1c1d7-p107">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="1c1d7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c1d7-146">Response</span></span>

<span data-ttu-id="1c1d7-147">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c1d7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1c1d7-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c1d7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c1d7-149">Request</span></span>
<span data-ttu-id="1c1d7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="1c1d7-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c1d7-151">Response</span></span>
<span data-ttu-id="1c1d7-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c1d7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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