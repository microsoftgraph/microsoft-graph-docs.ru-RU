---
title: Список столбцов
description: Получение списка объектов tablecolumn.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 69577701a2bd94bea50fa7619dc8c3261f4458d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876330"
---
# <a name="list-columns"></a><span data-ttu-id="b931a-103">Список столбцов</span><span class="sxs-lookup"><span data-stu-id="b931a-103">List columns</span></span>

> <span data-ttu-id="b931a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b931a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b931a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b931a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b931a-106">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="b931a-106">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b931a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b931a-107">Permissions</span></span>
<span data-ttu-id="b931a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b931a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b931a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b931a-110">Permission type</span></span>      | <span data-ttu-id="b931a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b931a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b931a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b931a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b931a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b931a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b931a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b931a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b931a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b931a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b931a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b931a-116">Application</span></span> | <span data-ttu-id="b931a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b931a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b931a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b931a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b931a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b931a-119">Optional query parameters</span></span>
<span data-ttu-id="b931a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b931a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="b931a-121">Для получения надежных результатов применяйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) на странице.</span><span class="sxs-lookup"><span data-stu-id="b931a-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="b931a-122">Это поможет избежать проблем с производительностью, связанных с большими результирующими наборами.</span><span class="sxs-lookup"><span data-stu-id="b931a-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b931a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b931a-123">Request headers</span></span>
| <span data-ttu-id="b931a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b931a-124">Name</span></span>      |<span data-ttu-id="b931a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b931a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b931a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b931a-126">Authorization</span></span>  | <span data-ttu-id="b931a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b931a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b931a-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b931a-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="b931a-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b931a-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b931a-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b931a-132">Request body</span></span>
<span data-ttu-id="b931a-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b931a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b931a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b931a-134">Response</span></span>

<span data-ttu-id="b931a-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b931a-135">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b931a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b931a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b931a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b931a-137">Request</span></span>
<span data-ttu-id="b931a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b931a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="b931a-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b931a-139">Response</span></span>
<span data-ttu-id="b931a-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b931a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```

> <span data-ttu-id="b931a-143">
  \*\*Примечание.\*\* Используйте параметры запросов [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) и [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter), чтобы просматривать постранично большое количество столбцов.</span><span class="sxs-lookup"><span data-stu-id="b931a-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="b931a-144">Пример.</span><span class="sxs-lookup"><span data-stu-id="b931a-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
