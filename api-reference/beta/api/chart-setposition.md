---
title: 'Chart: setPosition'
description: Располагает диаграмму относительно ячеек на листе.
ms.openlocfilehash: 8cb85aef81ac3399cf1b8825144dd889acebee66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075269"
---
# <a name="chart-setposition"></a><span data-ttu-id="ccd76-103">Chart: setPosition</span><span class="sxs-lookup"><span data-stu-id="ccd76-103">Chart: setPosition</span></span>

> <span data-ttu-id="ccd76-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ccd76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccd76-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccd76-106">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="ccd76-106">Positions the chart relative to cells on the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="ccd76-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd76-107">Permissions</span></span>
<span data-ttu-id="ccd76-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd76-110">Permission type</span></span>      | <span data-ttu-id="ccd76-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccd76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ccd76-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd76-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ccd76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd76-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccd76-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ccd76-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd76-116">Application</span></span> | <span data-ttu-id="ccd76-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd76-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccd76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setPosition

```
## <a name="request-headers"></a><span data-ttu-id="ccd76-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccd76-119">Request headers</span></span>
| <span data-ttu-id="ccd76-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ccd76-120">Name</span></span>       | <span data-ttu-id="ccd76-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd76-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ccd76-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccd76-122">Authorization</span></span>  | <span data-ttu-id="ccd76-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd76-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccd76-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ccd76-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ccd76-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ccd76-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd76-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccd76-128">Request body</span></span>
<span data-ttu-id="ccd76-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ccd76-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccd76-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ccd76-130">Parameter</span></span>    | <span data-ttu-id="ccd76-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd76-131">Type</span></span>   |<span data-ttu-id="ccd76-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd76-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccd76-133">startCell</span><span class="sxs-lookup"><span data-stu-id="ccd76-133">startCell</span></span>|<span data-ttu-id="ccd76-134">string</span><span class="sxs-lookup"><span data-stu-id="ccd76-134">string</span></span>|<span data-ttu-id="ccd76-p105">Начальная ячейка. Место, куда будет перемещена диаграмма. Начальная ячейка — это верхняя левая или верхняя правая ячейка (это зависит от того, использует ли пользователь параметры отображения справа налево).</span><span class="sxs-lookup"><span data-stu-id="ccd76-p105">The start cell. This is where the chart will be moved to. The start cell is the top-left or top-right cell, depending on the user's right-to-left display settings.</span></span>|
|<span data-ttu-id="ccd76-138">endCell</span><span class="sxs-lookup"><span data-stu-id="ccd76-138">endCell</span></span>|<span data-ttu-id="ccd76-139">string</span><span class="sxs-lookup"><span data-stu-id="ccd76-139">string</span></span>|<span data-ttu-id="ccd76-p106">Необязательный. Конечная ячейка. Если указан этот параметр, значения ширины и высоты диаграммы будут заданы так, чтобы полностью покрыть данную ячейку или диапазон.</span><span class="sxs-lookup"><span data-stu-id="ccd76-p106">Optional. The end cell. If specified, the chart's width and height will be set to fully cover up this cell/range.</span></span>|

## <a name="response"></a><span data-ttu-id="ccd76-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd76-143">Response</span></span>

<span data-ttu-id="ccd76-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ccd76-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd76-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd76-146">Example</span></span>
<span data-ttu-id="ccd76-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ccd76-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ccd76-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd76-148">Request</span></span>
<span data-ttu-id="ccd76-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd76-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ccd76-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccd76-150">Response</span></span>
<span data-ttu-id="ccd76-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd76-151">Here is an example of the response.</span></span> 
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