---
title: Обновление объекта chartAxis
description: Обновление свойств объекта chartaxis.
author: lumine2008
ms.openlocfilehash: bc6bea839751641530a3c3945307db2a206b7725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325489"
---
# <a name="update-chartaxis"></a><span data-ttu-id="199de-103">Обновление объекта chartAxis</span><span class="sxs-lookup"><span data-stu-id="199de-103">Update chartaxis</span></span>

> <span data-ttu-id="199de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="199de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="199de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="199de-106">Обновление свойств объекта chartaxis.</span><span class="sxs-lookup"><span data-stu-id="199de-106">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="199de-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="199de-107">Permissions</span></span>
<span data-ttu-id="199de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="199de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="199de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="199de-110">Permission type</span></span>      | <span data-ttu-id="199de-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="199de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="199de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="199de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="199de-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="199de-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="199de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="199de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="199de-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="199de-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="199de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="199de-116">Application</span></span> | <span data-ttu-id="199de-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="199de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="199de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="199de-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="199de-119">Optional request headers</span></span>
| <span data-ttu-id="199de-120">Имя</span><span class="sxs-lookup"><span data-stu-id="199de-120">Name</span></span>       | <span data-ttu-id="199de-121">Описание</span><span class="sxs-lookup"><span data-stu-id="199de-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="199de-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="199de-122">Authorization</span></span>  | <span data-ttu-id="199de-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="199de-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="199de-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="199de-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="199de-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="199de-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="199de-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="199de-128">Request body</span></span>
<span data-ttu-id="199de-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="199de-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="199de-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="199de-132">Property</span></span>     | <span data-ttu-id="199de-133">Тип</span><span class="sxs-lookup"><span data-stu-id="199de-133">Type</span></span>   |<span data-ttu-id="199de-134">Описание</span><span class="sxs-lookup"><span data-stu-id="199de-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="199de-135">majorUnit</span><span class="sxs-lookup"><span data-stu-id="199de-135">majorUnit</span></span>|<span data-ttu-id="199de-136">object</span><span class="sxs-lookup"><span data-stu-id="199de-136">object</span></span>|<span data-ttu-id="199de-p106">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="199de-p106">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="199de-140">maximum</span><span class="sxs-lookup"><span data-stu-id="199de-140">maximum</span></span>|<span data-ttu-id="199de-141">object</span><span class="sxs-lookup"><span data-stu-id="199de-141">object</span></span>|<span data-ttu-id="199de-p107">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="199de-p107">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="199de-145">minimum</span><span class="sxs-lookup"><span data-stu-id="199de-145">minimum</span></span>|<span data-ttu-id="199de-146">object</span><span class="sxs-lookup"><span data-stu-id="199de-146">object</span></span>|<span data-ttu-id="199de-p108">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="199de-p108">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="199de-150">minorUnit</span><span class="sxs-lookup"><span data-stu-id="199de-150">minorUnit</span></span>|<span data-ttu-id="199de-151">object</span><span class="sxs-lookup"><span data-stu-id="199de-151">object</span></span>|<span data-ttu-id="199de-p109">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="199de-p109">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="199de-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="199de-155">Response</span></span>

<span data-ttu-id="199de-156">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [ChartAxis](../resources/chartaxis.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="199de-156">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="199de-157">Пример</span><span class="sxs-lookup"><span data-stu-id="199de-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="199de-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="199de-158">Request</span></span>
<span data-ttu-id="199de-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="199de-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="199de-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="199de-160">Response</span></span>
<span data-ttu-id="199de-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="199de-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->