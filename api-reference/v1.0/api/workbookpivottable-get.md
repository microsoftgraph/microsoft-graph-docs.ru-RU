---
title: Получение workbookPivotTable
description: Получение свойств и связей объекта workbookPivotTable.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 660300bad2128c2436d1bca0301a7707e3c1b59b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805847"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="64fab-103">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="64fab-103">Get workbookPivotTable</span></span>

<span data-ttu-id="64fab-104">Получение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="64fab-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64fab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64fab-105">Permissions</span></span>
<span data-ttu-id="64fab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64fab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64fab-108">Permission type</span></span>      | <span data-ttu-id="64fab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64fab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64fab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64fab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64fab-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64fab-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64fab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64fab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64fab-113">Not supported.</span></span>    |
|<span data-ttu-id="64fab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64fab-114">Application</span></span> | <span data-ttu-id="64fab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64fab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64fab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64fab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64fab-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64fab-117">Optional query parameters</span></span>
<span data-ttu-id="64fab-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64fab-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64fab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64fab-119">Request headers</span></span>
| <span data-ttu-id="64fab-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64fab-120">Name</span></span>      |<span data-ttu-id="64fab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64fab-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64fab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64fab-122">Authorization</span></span>  | <span data-ttu-id="64fab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64fab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64fab-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="64fab-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="64fab-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="64fab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64fab-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64fab-128">Request body</span></span>
<span data-ttu-id="64fab-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64fab-129">Do not supply a request body for this method.</span></span>
### <a name="response"></a><span data-ttu-id="64fab-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="64fab-130">Response</span></span>
<span data-ttu-id="64fab-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64fab-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64fab-132">Пример</span><span class="sxs-lookup"><span data-stu-id="64fab-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64fab-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="64fab-133">Request</span></span>
<span data-ttu-id="64fab-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64fab-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="64fab-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="64fab-135">Response</span></span>
<span data-ttu-id="64fab-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64fab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```
