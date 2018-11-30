---
title: Получение объекта TableRow
description: Получение свойств и связей объекта tablerow.
ms.openlocfilehash: 330f29b58b05754f9feebac80a46c1b8745c70a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028166"
---
# <a name="get-tablerow"></a><span data-ttu-id="8d054-103">Получение объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="8d054-103">Get TableRow</span></span>

<span data-ttu-id="8d054-104">Получение свойств и связей объекта tablerow.</span><span class="sxs-lookup"><span data-stu-id="8d054-104">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d054-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d054-105">Permissions</span></span>
<span data-ttu-id="8d054-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d054-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d054-108">Permission type</span></span>      | <span data-ttu-id="8d054-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d054-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d054-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d054-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d054-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d054-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8d054-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d054-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d054-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d054-113">Not supported.</span></span>    |
|<span data-ttu-id="8d054-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d054-114">Application</span></span> | <span data-ttu-id="8d054-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d054-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d054-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d054-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d054-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d054-117">Optional query parameters</span></span>
<span data-ttu-id="8d054-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8d054-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d054-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d054-119">Request headers</span></span>
| <span data-ttu-id="8d054-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8d054-120">Name</span></span>      |<span data-ttu-id="8d054-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8d054-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d054-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d054-122">Authorization</span></span>  | <span data-ttu-id="8d054-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d054-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d054-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8d054-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8d054-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8d054-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d054-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d054-128">Request body</span></span>
<span data-ttu-id="8d054-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d054-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d054-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d054-130">Response</span></span>

<span data-ttu-id="8d054-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookTableRow](../resources/tablerow.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d054-131">If successful, this method returns a `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d054-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8d054-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d054-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d054-133">Request</span></span>
<span data-ttu-id="8d054-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d054-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```
##### <a name="response"></a><span data-ttu-id="8d054-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d054-135">Response</span></span>
<span data-ttu-id="8d054-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8d054-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->