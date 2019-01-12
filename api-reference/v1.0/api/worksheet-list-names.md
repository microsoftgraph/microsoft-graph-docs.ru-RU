---
title: Перечисление имен
description: 'Получение списка именованных элементов, связанных с листом. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4273ad75b012bf2884cd8b055c2fdb6e7e1abaff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927026"
---
# <a name="list-names"></a><span data-ttu-id="110ec-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="110ec-103">List names</span></span>

<span data-ttu-id="110ec-104">Получение списка именованных элементов, связанных с листом.</span><span class="sxs-lookup"><span data-stu-id="110ec-104">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="110ec-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="110ec-105">Permissions</span></span>
<span data-ttu-id="110ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="110ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="110ec-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="110ec-108">Permission type</span></span>      | <span data-ttu-id="110ec-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="110ec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="110ec-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="110ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="110ec-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="110ec-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="110ec-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="110ec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="110ec-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="110ec-113">Not supported.</span></span>    |
|<span data-ttu-id="110ec-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="110ec-114">Application</span></span> | <span data-ttu-id="110ec-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="110ec-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="110ec-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="110ec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="110ec-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="110ec-117">Optional query parameters</span></span>
<span data-ttu-id="110ec-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="110ec-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="110ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="110ec-119">Request headers</span></span>
| <span data-ttu-id="110ec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="110ec-120">Name</span></span>      |<span data-ttu-id="110ec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="110ec-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="110ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="110ec-122">Authorization</span></span>  | <span data-ttu-id="110ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="110ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="110ec-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="110ec-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="110ec-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="110ec-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="110ec-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="110ec-128">Request body</span></span>
<span data-ttu-id="110ec-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="110ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="110ec-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="110ec-130">Response</span></span>

<span data-ttu-id="110ec-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookNamedItem](../resources/nameditem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="110ec-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="110ec-132">Пример</span><span class="sxs-lookup"><span data-stu-id="110ec-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="110ec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="110ec-133">Request</span></span>
<span data-ttu-id="110ec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="110ec-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="110ec-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="110ec-135">Response</span></span>
<span data-ttu-id="110ec-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="110ec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
