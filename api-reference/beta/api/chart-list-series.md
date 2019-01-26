---
title: Список рядов
description: Получение списка объектов chartseries.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 69e84b83456d1c1f962e2c20bdadae81d9276917
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572138"
---
# <a name="list-series"></a><span data-ttu-id="b7594-103">Список рядов</span><span class="sxs-lookup"><span data-stu-id="b7594-103">List series</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7594-104">Получение списка объектов chartseries.</span><span class="sxs-lookup"><span data-stu-id="b7594-104">Retrieve a list of chartseries objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b7594-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7594-105">Permissions</span></span>
<span data-ttu-id="b7594-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7594-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7594-108">Permission type</span></span>      | <span data-ttu-id="b7594-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7594-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7594-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7594-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7594-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7594-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7594-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7594-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7594-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7594-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b7594-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7594-114">Application</span></span> | <span data-ttu-id="b7594-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7594-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7594-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7594-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7594-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7594-117">Optional query parameters</span></span>
<span data-ttu-id="b7594-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7594-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7594-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7594-119">Request headers</span></span>
| <span data-ttu-id="b7594-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b7594-120">Name</span></span>      |<span data-ttu-id="b7594-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b7594-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7594-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7594-122">Authorization</span></span>  | <span data-ttu-id="b7594-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7594-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b7594-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b7594-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b7594-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b7594-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7594-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7594-128">Request body</span></span>
<span data-ttu-id="b7594-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7594-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7594-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7594-130">Response</span></span>

<span data-ttu-id="b7594-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7594-131">If successful, this method returns a `200 OK` response code and collection of [ChartSeries](../resources/chartseries.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7594-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b7594-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7594-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7594-133">Request</span></span>
<span data-ttu-id="b7594-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7594-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_series"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
```
##### <a name="response"></a><span data-ttu-id="b7594-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7594-135">Response</span></span>
<span data-ttu-id="b7594-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b7594-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 59

{
  "value": [
    {
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List series",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-list-series.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
