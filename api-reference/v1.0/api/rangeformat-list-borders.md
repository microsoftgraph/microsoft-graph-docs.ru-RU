---
title: Список границ
description: Получение списка объектов rangeborder.
author: lumine2008
ms.openlocfilehash: 606dc6d3be61ca13d103cef496a2f34154de9b2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323893"
---
# <a name="list-borders"></a><span data-ttu-id="a73ea-103">Список границ</span><span class="sxs-lookup"><span data-stu-id="a73ea-103">List borders</span></span>

<span data-ttu-id="a73ea-104">Получение списка объектов rangeborder.</span><span class="sxs-lookup"><span data-stu-id="a73ea-104">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a73ea-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a73ea-105">Permissions</span></span>
<span data-ttu-id="a73ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a73ea-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a73ea-108">Permission type</span></span>      | <span data-ttu-id="a73ea-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a73ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a73ea-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a73ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a73ea-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a73ea-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a73ea-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a73ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a73ea-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73ea-113">Not supported.</span></span>    |
|<span data-ttu-id="a73ea-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a73ea-114">Application</span></span> | <span data-ttu-id="a73ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a73ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a73ea-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a73ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a73ea-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a73ea-117">Optional query parameters</span></span>
<span data-ttu-id="a73ea-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a73ea-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a73ea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a73ea-119">Request headers</span></span>
| <span data-ttu-id="a73ea-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a73ea-120">Name</span></span>      |<span data-ttu-id="a73ea-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a73ea-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a73ea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a73ea-122">Authorization</span></span>  | <span data-ttu-id="a73ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a73ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a73ea-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a73ea-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a73ea-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a73ea-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a73ea-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a73ea-128">Request body</span></span>
<span data-ttu-id="a73ea-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a73ea-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a73ea-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a73ea-130">Response</span></span>

<span data-ttu-id="a73ea-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookRangeBorder](../resources/rangeborder.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a73ea-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookRangeBorder](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a73ea-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a73ea-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a73ea-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a73ea-133">Request</span></span>
<span data-ttu-id="a73ea-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a73ea-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
```
##### <a name="response"></a><span data-ttu-id="a73ea-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a73ea-135">Response</span></span>
<span data-ttu-id="a73ea-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a73ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->