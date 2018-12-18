---
title: Список ChartPointsCollection
description: Получение списка объектов chartpoint.
author: lumine2008
ms.openlocfilehash: 1541e93505da09cbadb4434e4d24133f59a13de9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328219"
---
# <a name="list-chartpointscollection"></a><span data-ttu-id="e0a44-103">Список ChartPointsCollection</span><span class="sxs-lookup"><span data-stu-id="e0a44-103">List ChartPointsCollection</span></span>

> <span data-ttu-id="e0a44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0a44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0a44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0a44-106">Получение списка объектов chartpoint.</span><span class="sxs-lookup"><span data-stu-id="e0a44-106">Retrieve a list of chartpoint objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0a44-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a44-107">Permissions</span></span>
<span data-ttu-id="e0a44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a44-110">Permission type</span></span>      | <span data-ttu-id="e0a44-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0a44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0a44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0a44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0a44-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0a44-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0a44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0a44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a44-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0a44-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0a44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0a44-116">Application</span></span> | <span data-ttu-id="e0a44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a44-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0a44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0a44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0a44-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0a44-119">Optional query parameters</span></span>
<span data-ttu-id="e0a44-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0a44-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0a44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0a44-121">Request headers</span></span>
| <span data-ttu-id="e0a44-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e0a44-122">Name</span></span>      |<span data-ttu-id="e0a44-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a44-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0a44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0a44-124">Authorization</span></span>  | <span data-ttu-id="e0a44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0a44-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0a44-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0a44-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0a44-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e0a44-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0a44-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0a44-130">Request body</span></span>
<span data-ttu-id="e0a44-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0a44-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0a44-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a44-132">Response</span></span>

<span data-ttu-id="e0a44-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ChartPoint](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0a44-133">If successful, this method returns a `200 OK` response code and collection of [ChartPoint](../resources/chartpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0a44-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e0a44-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0a44-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0a44-135">Request</span></span>
<span data-ttu-id="e0a44-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0a44-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartpointscollection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
```
##### <a name="response"></a><span data-ttu-id="e0a44-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0a44-137">Response</span></span>
<span data-ttu-id="e0a44-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e0a44-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 57

{
  "value": [
    {
      "value": {
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartPointsCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->