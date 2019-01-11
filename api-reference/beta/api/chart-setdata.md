---
title: 'Chart: setData'
description: Сбрасывает исходные данные для диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 83d74036019ffe1f58e86778859d5123dc3df8c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883757"
---
# <a name="chart-setdata"></a><span data-ttu-id="7ac3b-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="7ac3b-103">Chart: setData</span></span>

> <span data-ttu-id="7ac3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ac3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ac3b-106">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-106">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ac3b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ac3b-107">Permissions</span></span>
<span data-ttu-id="7ac3b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ac3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ac3b-110">Permission type</span></span>      | <span data-ttu-id="7ac3b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ac3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ac3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ac3b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ac3b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ac3b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ac3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ac3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ac3b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ac3b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ac3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ac3b-116">Application</span></span> | <span data-ttu-id="7ac3b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ac3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ac3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/setData

```
## <a name="request-headers"></a><span data-ttu-id="7ac3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ac3b-119">Request headers</span></span>
| <span data-ttu-id="7ac3b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7ac3b-120">Name</span></span>       | <span data-ttu-id="7ac3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac3b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7ac3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ac3b-122">Authorization</span></span>  | <span data-ttu-id="7ac3b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ac3b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7ac3b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ac3b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac3b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ac3b-128">Request body</span></span>
<span data-ttu-id="7ac3b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7ac3b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7ac3b-130">Parameter</span></span>    | <span data-ttu-id="7ac3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac3b-131">Type</span></span>   |<span data-ttu-id="7ac3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac3b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ac3b-133">sourceData</span><span class="sxs-lookup"><span data-stu-id="7ac3b-133">sourceData</span></span>|<span data-ttu-id="7ac3b-134">string</span><span class="sxs-lookup"><span data-stu-id="7ac3b-134">string</span></span>|<span data-ttu-id="7ac3b-135">Объект Range, соответствующий исходным данным.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-135">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="7ac3b-136">seriesBy</span><span class="sxs-lookup"><span data-stu-id="7ac3b-136">seriesBy</span></span>|<span data-ttu-id="7ac3b-137">string</span><span class="sxs-lookup"><span data-stu-id="7ac3b-137">string</span></span>|<span data-ttu-id="7ac3b-p105">Необязательный параметр. Определяет способ использования столбцов или строк в качестве рядов данных на диаграмме. Может иметь одно из следующих значений: Auto (по умолчанию), Rows, Columns.  Возможные значения: `Auto`, `Columns`, `Rows`.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-p105">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="7ac3b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ac3b-142">Response</span></span>

<span data-ttu-id="7ac3b-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac3b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="7ac3b-145">Example</span></span>
<span data-ttu-id="7ac3b-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7ac3b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ac3b-147">Request</span></span>
<span data-ttu-id="7ac3b-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="7ac3b-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ac3b-149">Response</span></span>
<span data-ttu-id="7ac3b-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ac3b-150">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
