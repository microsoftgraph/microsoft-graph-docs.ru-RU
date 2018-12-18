---
title: Обновление объекта ChartLineFormat
description: Обновление свойств объекта chartlineformat.
author: lumine2008
ms.openlocfilehash: 816056cefea715317a05d65eebf696c2cc907cfe
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316445"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="a5a02-103">Обновление объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a5a02-103">Update chartlineformat</span></span>

> <span data-ttu-id="a5a02-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5a02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5a02-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5a02-106">Обновление свойств объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="a5a02-106">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a5a02-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a02-107">Permissions</span></span>
<span data-ttu-id="a5a02-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a02-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a02-110">Permission type</span></span>      | <span data-ttu-id="a5a02-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5a02-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5a02-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5a02-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a5a02-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5a02-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5a02-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a5a02-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5a02-116">Application</span></span> | <span data-ttu-id="a5a02-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a02-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5a02-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="a5a02-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a02-119">Optional request headers</span></span>
| <span data-ttu-id="a5a02-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a5a02-120">Name</span></span>       | <span data-ttu-id="a5a02-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a02-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5a02-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5a02-122">Authorization</span></span>  | <span data-ttu-id="a5a02-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5a02-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5a02-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a5a02-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a5a02-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a5a02-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5a02-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5a02-128">Request body</span></span>
<span data-ttu-id="a5a02-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a5a02-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5a02-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5a02-132">Property</span></span>     | <span data-ttu-id="a5a02-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a5a02-133">Type</span></span>   |<span data-ttu-id="a5a02-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a02-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5a02-135">color</span><span class="sxs-lookup"><span data-stu-id="a5a02-135">color</span></span>|<span data-ttu-id="a5a02-136">строка</span><span class="sxs-lookup"><span data-stu-id="a5a02-136">string</span></span>|<span data-ttu-id="a5a02-137">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a5a02-137">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="a5a02-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a02-138">Response</span></span>

<span data-ttu-id="a5a02-139">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartLineFormat](../resources/chartlineformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a5a02-139">If successful, this method returns a `200 OK` response code and updated [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5a02-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a5a02-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5a02-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a02-141">Request</span></span>
<span data-ttu-id="a5a02-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a02-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="a5a02-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5a02-143">Response</span></span>
<span data-ttu-id="a5a02-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a5a02-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLineFormat"
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