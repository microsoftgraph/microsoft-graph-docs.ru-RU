---
title: Список строк
description: Получение списка объектов tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 46d121e1555cad780d12fa6922d6aa3867cc792e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524998"
---
# <a name="list-rows"></a><span data-ttu-id="cec42-103">Список строк</span><span class="sxs-lookup"><span data-stu-id="cec42-103">List rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cec42-104">Получение списка объектов tablerow.</span><span class="sxs-lookup"><span data-stu-id="cec42-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cec42-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cec42-105">Permissions</span></span>
<span data-ttu-id="cec42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cec42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec42-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cec42-108">Permission type</span></span>      | <span data-ttu-id="cec42-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cec42-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cec42-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cec42-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cec42-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cec42-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cec42-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cec42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cec42-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cec42-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cec42-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cec42-114">Application</span></span> | <span data-ttu-id="cec42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cec42-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cec42-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cec42-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cec42-117">Optional query parameters</span></span>
<span data-ttu-id="cec42-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cec42-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="cec42-119">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="cec42-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="cec42-120">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="cec42-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cec42-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cec42-121">Request headers</span></span>
| <span data-ttu-id="cec42-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cec42-122">Name</span></span>      |<span data-ttu-id="cec42-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cec42-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cec42-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cec42-124">Authorization</span></span>  | <span data-ttu-id="cec42-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cec42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cec42-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cec42-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="cec42-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cec42-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec42-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cec42-130">Request body</span></span>
<span data-ttu-id="cec42-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cec42-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cec42-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec42-132">Response</span></span>

<span data-ttu-id="cec42-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cec42-133">If successful, this method returns a `200 OK` response code and collection of [TableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cec42-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cec42-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cec42-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cec42-135">Request</span></span>
<span data-ttu-id="cec42-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cec42-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="cec42-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="cec42-137">Response</span></span>
<span data-ttu-id="cec42-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cec42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="cec42-141">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter), чтобы просматривать постранично большое количество строк.</span><span class="sxs-lookup"><span data-stu-id="cec42-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="cec42-142">Пример.</span><span class="sxs-lookup"><span data-stu-id="cec42-142">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
