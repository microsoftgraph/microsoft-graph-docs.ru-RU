---
title: Получение объекта Chart
description: Получение свойств и связей объекта диаграммы.
ms.openlocfilehash: db6fc68c50ef608e4ee81a576911499039676b63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027416"
---
# <a name="get-chart"></a><span data-ttu-id="c2d30-103">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="c2d30-103">Get Chart</span></span>

<span data-ttu-id="c2d30-104">Получение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c2d30-104">Retrieve the properties and relationships of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2d30-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2d30-105">Permissions</span></span>
<span data-ttu-id="c2d30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2d30-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2d30-108">Permission type</span></span>      | <span data-ttu-id="c2d30-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2d30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2d30-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2d30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2d30-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2d30-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2d30-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2d30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2d30-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d30-113">Not supported.</span></span>    |
|<span data-ttu-id="c2d30-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2d30-114">Application</span></span> | <span data-ttu-id="c2d30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d30-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2d30-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2d30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2d30-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2d30-117">Optional query parameters</span></span>
<span data-ttu-id="c2d30-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2d30-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2d30-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2d30-119">Request headers</span></span>
| <span data-ttu-id="c2d30-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c2d30-120">Name</span></span>      |<span data-ttu-id="c2d30-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d30-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2d30-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2d30-122">Authorization</span></span>  | <span data-ttu-id="c2d30-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2d30-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2d30-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c2d30-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c2d30-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c2d30-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2d30-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2d30-128">Request body</span></span>
<span data-ttu-id="c2d30-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2d30-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2d30-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2d30-130">Response</span></span>

<span data-ttu-id="c2d30-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookChart](../resources/chart.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2d30-131">If successful, this method returns a `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2d30-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c2d30-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2d30-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2d30-133">Request</span></span>
<span data-ttu-id="c2d30-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2d30-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chart"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```
##### <a name="response"></a><span data-ttu-id="c2d30-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2d30-135">Response</span></span>
<span data-ttu-id="c2d30-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c2d30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->