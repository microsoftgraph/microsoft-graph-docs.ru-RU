---
title: Получение объекта ChartDataLabels
description: Получение свойств и связей объекта chartdatalabels.
ms.openlocfilehash: fa1146bb08336c4d44bd4f44ddedd789ef0768b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074982"
---
# <a name="get-chartdatalabels"></a><span data-ttu-id="c03bb-103">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c03bb-103">Get ChartDataLabels</span></span>

> <span data-ttu-id="c03bb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c03bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c03bb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c03bb-106">Получение свойств и связей объекта chartdatalabels.</span><span class="sxs-lookup"><span data-stu-id="c03bb-106">Retrieve the properties and relationships of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c03bb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c03bb-107">Permissions</span></span>
<span data-ttu-id="c03bb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c03bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c03bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c03bb-110">Permission type</span></span>      | <span data-ttu-id="c03bb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c03bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c03bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c03bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c03bb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c03bb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c03bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c03bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c03bb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c03bb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c03bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c03bb-116">Application</span></span> | <span data-ttu-id="c03bb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03bb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c03bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c03bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c03bb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c03bb-119">Optional query parameters</span></span>
<span data-ttu-id="c03bb-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c03bb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c03bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c03bb-121">Request headers</span></span>
| <span data-ttu-id="c03bb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c03bb-122">Name</span></span>      |<span data-ttu-id="c03bb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c03bb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c03bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c03bb-124">Authorization</span></span>  | <span data-ttu-id="c03bb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c03bb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c03bb-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c03bb-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="c03bb-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c03bb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c03bb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c03bb-130">Request body</span></span>
<span data-ttu-id="c03bb-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c03bb-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c03bb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c03bb-132">Response</span></span>

<span data-ttu-id="c03bb-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartDataLabels](../resources/chartdatalabels.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c03bb-133">If successful, this method returns a `200 OK` response code and [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c03bb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c03bb-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c03bb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c03bb-135">Request</span></span>
<span data-ttu-id="c03bb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c03bb-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartdatalabels"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
##### <a name="response"></a><span data-ttu-id="c03bb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c03bb-137">Response</span></span>
<span data-ttu-id="c03bb-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c03bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartDataLabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->