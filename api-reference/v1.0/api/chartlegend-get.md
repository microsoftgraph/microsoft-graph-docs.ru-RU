---
title: Получение объекта ChartLegend
description: Получение свойств и связей объекта chartlegend.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2b29b3a4a83070000693c23bcfc6d7df001b17f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835331"
---
# <a name="get-chartlegend"></a><span data-ttu-id="e9362-103">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="e9362-103">Get ChartLegend</span></span>

<span data-ttu-id="e9362-104">Получение свойств и связей объекта chartlegend.</span><span class="sxs-lookup"><span data-stu-id="e9362-104">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9362-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9362-105">Permissions</span></span>
<span data-ttu-id="e9362-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9362-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9362-108">Permission type</span></span>      | <span data-ttu-id="e9362-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9362-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9362-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9362-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9362-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9362-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9362-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9362-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9362-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9362-113">Not supported.</span></span>    |
|<span data-ttu-id="e9362-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9362-114">Application</span></span> | <span data-ttu-id="e9362-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9362-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9362-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9362-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9362-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9362-117">Optional query parameters</span></span>
<span data-ttu-id="e9362-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9362-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9362-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9362-119">Request headers</span></span>
| <span data-ttu-id="e9362-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e9362-120">Name</span></span>      |<span data-ttu-id="e9362-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e9362-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9362-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9362-122">Authorization</span></span>  | <span data-ttu-id="e9362-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9362-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9362-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9362-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9362-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e9362-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9362-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9362-128">Request body</span></span>
<span data-ttu-id="e9362-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9362-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9362-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9362-130">Response</span></span>

<span data-ttu-id="e9362-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookChartLegend](../resources/chartlegend.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9362-131">If successful, this method returns a `200 OK` response code and [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9362-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e9362-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9362-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9362-133">Request</span></span>
<span data-ttu-id="e9362-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9362-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartlegend"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
```
##### <a name="response"></a><span data-ttu-id="e9362-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9362-135">Response</span></span>
<span data-ttu-id="e9362-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9362-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartLegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
