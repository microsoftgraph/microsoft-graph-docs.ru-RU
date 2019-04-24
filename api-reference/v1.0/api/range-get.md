---
title: Получение объекта Range
description: Получение свойств и связей объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7d7f12c4a2bbc40cf43be325dd0a600ff0c4ee4d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453325"
---
# <a name="get-range"></a><span data-ttu-id="687ca-103">Получение объекта Range</span><span class="sxs-lookup"><span data-stu-id="687ca-103">Get Range</span></span>

<span data-ttu-id="687ca-104">Получение свойств и связей объекта диапазона.</span><span class="sxs-lookup"><span data-stu-id="687ca-104">Retrieve the properties and relationships of range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="687ca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="687ca-105">Permissions</span></span>
<span data-ttu-id="687ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="687ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687ca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="687ca-108">Permission type</span></span>      | <span data-ttu-id="687ca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="687ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="687ca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="687ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="687ca-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="687ca-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="687ca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="687ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="687ca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="687ca-113">Not supported.</span></span>    |
|<span data-ttu-id="687ca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="687ca-114">Application</span></span> | <span data-ttu-id="687ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="687ca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="687ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="687ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range(address='<address>')
GET /workbook/tables/{id|name}/columns/{id|name}/range
```
## <a name="optional-query-parameters"></a><span data-ttu-id="687ca-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="687ca-117">Optional query parameters</span></span>
<span data-ttu-id="687ca-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="687ca-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="687ca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="687ca-119">Request headers</span></span>
| <span data-ttu-id="687ca-120">Имя</span><span class="sxs-lookup"><span data-stu-id="687ca-120">Name</span></span>      |<span data-ttu-id="687ca-121">Описание</span><span class="sxs-lookup"><span data-stu-id="687ca-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="687ca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="687ca-122">Authorization</span></span>  | <span data-ttu-id="687ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="687ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="687ca-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="687ca-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="687ca-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="687ca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="687ca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="687ca-128">Request body</span></span>
<span data-ttu-id="687ca-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="687ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="687ca-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="687ca-130">Response</span></span>

<span data-ttu-id="687ca-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="687ca-131">If successful, this method returns a `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="687ca-132">Пример</span><span class="sxs-lookup"><span data-stu-id="687ca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="687ca-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="687ca-133">Request</span></span>
<span data-ttu-id="687ca-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="687ca-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
##### <a name="response"></a><span data-ttu-id="687ca-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="687ca-135">Response</span></span>
<span data-ttu-id="687ca-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="687ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
