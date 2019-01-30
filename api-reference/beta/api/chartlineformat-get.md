---
title: Получение объекта ChartLineFormat
description: Получение свойств и связей объекта chartlineformat.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a84e0d9c31f08ac8fe6396cb73e2fd7fb0993e0c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643939"
---
# <a name="get-chartlineformat"></a><span data-ttu-id="f777a-103">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="f777a-103">Get ChartLineFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f777a-104">Получение свойств и связей объекта chartlineformat.</span><span class="sxs-lookup"><span data-stu-id="f777a-104">Retrieve the properties and relationships of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f777a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f777a-105">Permissions</span></span>
<span data-ttu-id="f777a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f777a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f777a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f777a-108">Permission type</span></span>      | <span data-ttu-id="f777a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f777a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f777a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f777a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f777a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f777a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f777a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f777a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f777a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f777a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f777a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f777a-114">Application</span></span> | <span data-ttu-id="f777a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f777a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f777a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f777a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis/format/line
GET /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/majorgridlines/format/line
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f777a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f777a-117">Optional query parameters</span></span>
<span data-ttu-id="f777a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f777a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f777a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f777a-119">Request headers</span></span>
| <span data-ttu-id="f777a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f777a-120">Name</span></span>      |<span data-ttu-id="f777a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f777a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f777a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f777a-122">Authorization</span></span>  | <span data-ttu-id="f777a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f777a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f777a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f777a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f777a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f777a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f777a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f777a-128">Request body</span></span>
<span data-ttu-id="f777a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f777a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f777a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f777a-130">Response</span></span>

<span data-ttu-id="f777a-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [ChartLineFormat](../resources/chartlineformat.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f777a-131">If successful, this method returns a `200 OK` response code and [ChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f777a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f777a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f777a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f777a-133">Request</span></span>
<span data-ttu-id="f777a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f777a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartlineformat"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis/format/line
```
##### <a name="response"></a><span data-ttu-id="f777a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f777a-135">Response</span></span>
<span data-ttu-id="f777a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f777a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartLineFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartlineformat-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
