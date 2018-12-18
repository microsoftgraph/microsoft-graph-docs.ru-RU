---
title: Получение workbookPivotTable
description: Получение свойств и связей объекта workbookPivotTable.
author: lumine2008
ms.openlocfilehash: 00f994fcbffeb8214a6326130746c0200c162107
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344894"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="4e26c-103">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="4e26c-103">Get workbookPivotTable</span></span>

> <span data-ttu-id="4e26c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e26c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e26c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e26c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e26c-106">Получение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="4e26c-106">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e26c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e26c-107">Permissions</span></span>
<span data-ttu-id="4e26c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e26c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e26c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e26c-110">Permission type</span></span>      | <span data-ttu-id="4e26c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e26c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e26c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e26c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e26c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e26c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e26c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e26c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e26c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e26c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e26c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e26c-116">Application</span></span> | <span data-ttu-id="4e26c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e26c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e26c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e26c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e26c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e26c-119">Optional query parameters</span></span>
<span data-ttu-id="4e26c-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e26c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e26c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e26c-121">Request headers</span></span>
| <span data-ttu-id="4e26c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4e26c-122">Name</span></span>      |<span data-ttu-id="4e26c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4e26c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e26c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e26c-124">Authorization</span></span>  | <span data-ttu-id="4e26c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e26c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e26c-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e26c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e26c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e26c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e26c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e26c-130">Request body</span></span>
<span data-ttu-id="4e26c-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e26c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e26c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e26c-132">Response</span></span>

<span data-ttu-id="4e26c-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e26c-133">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e26c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="4e26c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e26c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e26c-135">Request</span></span>
<span data-ttu-id="4e26c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e26c-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="4e26c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e26c-137">Response</span></span>
<span data-ttu-id="4e26c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4e26c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
