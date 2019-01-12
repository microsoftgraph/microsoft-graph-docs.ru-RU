---
title: Список ChartCollection
description: Получение списка объектов диаграмм.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6735974929faf06c0359c2f99d99f4a1cf460507
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930252"
---
# <a name="list-chartcollection"></a><span data-ttu-id="b582c-103">Список ChartCollection</span><span class="sxs-lookup"><span data-stu-id="b582c-103">List ChartCollection</span></span>

<span data-ttu-id="b582c-104">Получение списка объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="b582c-104">Retrieve a list of chart objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b582c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b582c-105">Permissions</span></span>
<span data-ttu-id="b582c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b582c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b582c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b582c-108">Permission type</span></span>      | <span data-ttu-id="b582c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b582c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b582c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b582c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b582c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b582c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b582c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b582c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b582c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b582c-113">Not supported.</span></span>    |
|<span data-ttu-id="b582c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b582c-114">Application</span></span> | <span data-ttu-id="b582c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b582c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b582c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b582c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b582c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b582c-117">Optional query parameters</span></span>
<span data-ttu-id="b582c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b582c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b582c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b582c-119">Request headers</span></span>
| <span data-ttu-id="b582c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b582c-120">Name</span></span>      |<span data-ttu-id="b582c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b582c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b582c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b582c-122">Authorization</span></span>  | <span data-ttu-id="b582c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b582c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b582c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b582c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b582c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b582c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b582c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b582c-128">Request body</span></span>
<span data-ttu-id="b582c-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b582c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b582c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b582c-130">Response</span></span>

<span data-ttu-id="b582c-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookChart](../resources/chart.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b582c-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookChart](../resources/chart.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b582c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b582c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b582c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b582c-133">Request</span></span>
<span data-ttu-id="b582c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b582c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
```
##### <a name="response"></a><span data-ttu-id="b582c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b582c-135">Response</span></span>
<span data-ttu-id="b582c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b582c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 93

{
  "value": [
    {
      "id": "id-value",
      "height": 99,
      "left": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List ChartCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
