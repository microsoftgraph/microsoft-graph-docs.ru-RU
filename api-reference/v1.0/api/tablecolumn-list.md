---
title: Список TableColumnCollection
description: Получение списка объектов tablecolumn.
author: lumine2008
ms.openlocfilehash: b050d9e322df9aa6f6a07d509ccf7a17637e77e6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309543"
---
# <a name="list-tablecolumncollection"></a><span data-ttu-id="8b669-103">Список TableColumnCollection</span><span class="sxs-lookup"><span data-stu-id="8b669-103">List TableColumnCollection</span></span>

<span data-ttu-id="8b669-104">Получение списка объектов tablecolumn.</span><span class="sxs-lookup"><span data-stu-id="8b669-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b669-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b669-105">Permissions</span></span>
<span data-ttu-id="8b669-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b669-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b669-108">Permission type</span></span>      | <span data-ttu-id="8b669-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b669-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b669-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b669-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b669-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b669-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b669-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b669-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b669-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b669-113">Not supported.</span></span>    |
|<span data-ttu-id="8b669-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b669-114">Application</span></span> | <span data-ttu-id="8b669-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b669-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b669-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b669-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b669-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b669-117">Optional query parameters</span></span>
<span data-ttu-id="8b669-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b669-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b669-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b669-119">Request headers</span></span>
| <span data-ttu-id="8b669-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8b669-120">Name</span></span>      |<span data-ttu-id="8b669-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8b669-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b669-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b669-122">Authorization</span></span>  | <span data-ttu-id="8b669-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b669-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b669-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b669-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b669-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8b669-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b669-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b669-128">Request body</span></span>
<span data-ttu-id="8b669-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b669-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b669-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b669-130">Response</span></span>

<span data-ttu-id="8b669-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookTableColumn](../resources/tablecolumn.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b669-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b669-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8b669-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b669-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b669-133">Request</span></span>
<span data-ttu-id="8b669-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b669-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecolumncollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
```
##### <a name="response"></a><span data-ttu-id="8b669-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b669-135">Response</span></span>
<span data-ttu-id="8b669-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8b669-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableColumnCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->