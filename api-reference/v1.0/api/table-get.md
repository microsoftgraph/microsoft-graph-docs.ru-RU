---
title: Получение объекта Table
description: Получение свойств и связей объекта таблицы.
author: lumine2008
ms.openlocfilehash: 57e3c88cb2a483bb567095a59769e770ae974edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353398"
---
# <a name="get-table"></a><span data-ttu-id="6ef5a-103">Получение объекта Table</span><span class="sxs-lookup"><span data-stu-id="6ef5a-103">Get Table</span></span>

<span data-ttu-id="6ef5a-104">Получение свойств и связей объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-104">Retrieve the properties and relationships of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ef5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef5a-105">Permissions</span></span>
<span data-ttu-id="6ef5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ef5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ef5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef5a-108">Permission type</span></span>      | <span data-ttu-id="6ef5a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ef5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ef5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ef5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ef5a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ef5a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ef5a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ef5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef5a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-113">Not supported.</span></span>    |
|<span data-ttu-id="6ef5a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ef5a-114">Application</span></span> | <span data-ttu-id="6ef5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ef5a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ef5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}
GET /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ef5a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ef5a-117">Optional query parameters</span></span>
<span data-ttu-id="6ef5a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ef5a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ef5a-119">Request headers</span></span>
| <span data-ttu-id="6ef5a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ef5a-120">Name</span></span>      |<span data-ttu-id="6ef5a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef5a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ef5a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ef5a-122">Authorization</span></span>  | <span data-ttu-id="6ef5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ef5a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ef5a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ef5a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ef5a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ef5a-128">Request body</span></span>
<span data-ttu-id="6ef5a-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ef5a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ef5a-130">Response</span></span>

<span data-ttu-id="6ef5a-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookTable](../resources/table.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-131">If successful, this method returns a `200 OK` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ef5a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6ef5a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ef5a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef5a-133">Request</span></span>
<span data-ttu-id="6ef5a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_table"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
```
##### <a name="response"></a><span data-ttu-id="6ef5a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ef5a-135">Response</span></span>
<span data-ttu-id="6ef5a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6ef5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
