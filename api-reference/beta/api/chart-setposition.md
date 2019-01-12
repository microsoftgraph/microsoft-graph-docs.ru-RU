---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: dae44414db5a095c4cf12506582a9533972a0373
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941221"
---
# <a name="chart-setposition"></a><span data-ttu-id="bf4d0-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="bf4d0-103">Chart: setPosition</span></span>

> <span data-ttu-id="bf4d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf4d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf4d0-106">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="bf4d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4d0-107">Permissions</span></span>
<span data-ttu-id="bf4d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4d0-110">Permission type</span></span>      | <span data-ttu-id="bf4d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf4d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf4d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf4d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf4d0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4d0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf4d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf4d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf4d0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4d0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bf4d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf4d0-116">Application</span></span> | <span data-ttu-id="bf4d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf4d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf4d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="bf4d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf4d0-119">Request headers</span></span>
| <span data-ttu-id="bf4d0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bf4d0-120">Name</span></span>       | <span data-ttu-id="bf4d0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4d0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bf4d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf4d0-122">Authorization</span></span>  | <span data-ttu-id="bf4d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf4d0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bf4d0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bf4d0-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf4d0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf4d0-128">Request body</span></span>
<span data-ttu-id="bf4d0-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bf4d0-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="bf4d0-130">Parameter</span></span>    | <span data-ttu-id="bf4d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf4d0-131">Type</span></span>   |<span data-ttu-id="bf4d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4d0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf4d0-133">startCell</span><span class="sxs-lookup"><span data-stu-id="bf4d0-133">startCell</span></span>|<span data-ttu-id="bf4d0-134">string</span><span class="sxs-lookup"><span data-stu-id="bf4d0-134">string</span></span>|<span data-ttu-id="bf4d0-p105">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="bf4d0-138">endCell</span><span class="sxs-lookup"><span data-stu-id="bf4d0-138">endCell</span></span>|<span data-ttu-id="bf4d0-139">string</span><span class="sxs-lookup"><span data-stu-id="bf4d0-139">string</span></span>|<span data-ttu-id="bf4d0-p106">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="bf4d0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4d0-143">Response</span></span>

<span data-ttu-id="bf4d0-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf4d0-146">Пример</span><span class="sxs-lookup"><span data-stu-id="bf4d0-146">Example</span></span>
<span data-ttu-id="bf4d0-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bf4d0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf4d0-148">Request</span></span>
<span data-ttu-id="bf4d0-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setposition"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setPosition
Content-type: application/json
Content-length: 66

{
  "startCell": "startCell-value",
  "endCell": "endCell-value"
}
```

##### <a name="response"></a><span data-ttu-id="bf4d0-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf4d0-150">Response</span></span>
<span data-ttu-id="bf4d0-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf4d0-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: setPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
