---
title: Получение списка pivotTables
description: Получение списка объектов workbookpivottable.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c9aac1b23045ee6f6e751e75dccdc57f61a95203
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845229"
---
# <a name="list-pivottables"></a><span data-ttu-id="99ffd-103">Получение списка pivotTables</span><span class="sxs-lookup"><span data-stu-id="99ffd-103">List pivotTables</span></span>

> <span data-ttu-id="99ffd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99ffd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ffd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99ffd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ffd-106">Получение списка объектов workbookpivottable.</span><span class="sxs-lookup"><span data-stu-id="99ffd-106">Retrieve a list of workbookpivottable objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="99ffd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99ffd-107">Permissions</span></span>
<span data-ttu-id="99ffd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99ffd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="99ffd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99ffd-110">Permission type</span></span>      | <span data-ttu-id="99ffd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99ffd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99ffd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99ffd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99ffd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ffd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99ffd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99ffd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99ffd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ffd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99ffd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99ffd-116">Application</span></span> | <span data-ttu-id="99ffd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99ffd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99ffd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99ffd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99ffd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99ffd-119">Optional query parameters</span></span>
<span data-ttu-id="99ffd-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="99ffd-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99ffd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99ffd-121">Request headers</span></span>
| <span data-ttu-id="99ffd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="99ffd-122">Name</span></span>      |<span data-ttu-id="99ffd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="99ffd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99ffd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99ffd-124">Authorization</span></span>  | <span data-ttu-id="99ffd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99ffd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99ffd-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99ffd-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="99ffd-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="99ffd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99ffd-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99ffd-130">Request body</span></span>
<span data-ttu-id="99ffd-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99ffd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99ffd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="99ffd-132">Response</span></span>

<span data-ttu-id="99ffd-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99ffd-133">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99ffd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="99ffd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99ffd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="99ffd-135">Request</span></span>
<span data-ttu-id="99ffd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99ffd-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_pivottables"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables
```
##### <a name="response"></a><span data-ttu-id="99ffd-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="99ffd-137">Response</span></span>
<span data-ttu-id="99ffd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="99ffd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookPivotTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```
