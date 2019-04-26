---
title: Получение workbookPivotTable
description: Получение свойств и связей объекта workbookPivotTable.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 458d2f065af512b4bc33481916085fecf50aa4af
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339517"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="848ff-103">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="848ff-103">Get workbookPivotTable</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="848ff-104">Получение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="848ff-104">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="848ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="848ff-105">Permissions</span></span>
<span data-ttu-id="848ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="848ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="848ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="848ff-108">Permission type</span></span>      | <span data-ttu-id="848ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="848ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="848ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="848ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="848ff-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848ff-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="848ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="848ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="848ff-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="848ff-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="848ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="848ff-114">Application</span></span> | <span data-ttu-id="848ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="848ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="848ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="848ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="848ff-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="848ff-117">Optional query parameters</span></span>
<span data-ttu-id="848ff-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="848ff-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="848ff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="848ff-119">Request headers</span></span>
| <span data-ttu-id="848ff-120">Имя</span><span class="sxs-lookup"><span data-stu-id="848ff-120">Name</span></span>      |<span data-ttu-id="848ff-121">Описание</span><span class="sxs-lookup"><span data-stu-id="848ff-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="848ff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="848ff-122">Authorization</span></span>  | <span data-ttu-id="848ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="848ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="848ff-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="848ff-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="848ff-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="848ff-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="848ff-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="848ff-128">Request body</span></span>
<span data-ttu-id="848ff-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="848ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="848ff-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="848ff-130">Response</span></span>

<span data-ttu-id="848ff-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="848ff-131">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="848ff-132">Пример</span><span class="sxs-lookup"><span data-stu-id="848ff-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="848ff-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="848ff-133">Request</span></span>
<span data-ttu-id="848ff-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="848ff-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="848ff-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="848ff-135">Response</span></span>
<span data-ttu-id="848ff-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="848ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
