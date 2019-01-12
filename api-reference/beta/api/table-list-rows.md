---
title: Список строк
description: Получение списка объектов tablerow.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d5edeb8027a7e6d75af2244fce988eac92c2edc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970152"
---
# <a name="list-rows"></a><span data-ttu-id="4c041-103">Список строк</span><span class="sxs-lookup"><span data-stu-id="4c041-103">List rows</span></span>

> <span data-ttu-id="4c041-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c041-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c041-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c041-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c041-106">Получение списка объектов tablerow.</span><span class="sxs-lookup"><span data-stu-id="4c041-106">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c041-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c041-107">Permissions</span></span>
<span data-ttu-id="4c041-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c041-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c041-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c041-110">Permission type</span></span>      | <span data-ttu-id="4c041-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c041-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c041-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c041-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c041-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c041-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4c041-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c041-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c041-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c041-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4c041-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c041-116">Application</span></span> | <span data-ttu-id="4c041-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c041-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c041-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c041-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c041-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c041-119">Optional query parameters</span></span>
<span data-ttu-id="4c041-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c041-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="4c041-121">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="4c041-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="4c041-122">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="4c041-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c041-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c041-123">Request headers</span></span>
| <span data-ttu-id="4c041-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4c041-124">Name</span></span>      |<span data-ttu-id="4c041-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4c041-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c041-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c041-126">Authorization</span></span>  | <span data-ttu-id="4c041-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c041-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c041-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4c041-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="4c041-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4c041-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c041-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c041-132">Request body</span></span>
<span data-ttu-id="4c041-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c041-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c041-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c041-134">Response</span></span>

<span data-ttu-id="4c041-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c041-135">If successful, this method returns a `200 OK` response code and collection of [TableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c041-136">Пример</span><span class="sxs-lookup"><span data-stu-id="4c041-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c041-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c041-137">Request</span></span>
<span data-ttu-id="4c041-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c041-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="4c041-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c041-139">Response</span></span>
<span data-ttu-id="4c041-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c041-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="4c041-143">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter), чтобы просматривать постранично большое количество строк.</span><span class="sxs-lookup"><span data-stu-id="4c041-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="4c041-144">Пример.</span><span class="sxs-lookup"><span data-stu-id="4c041-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
