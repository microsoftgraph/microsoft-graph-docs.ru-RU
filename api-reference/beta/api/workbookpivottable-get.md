---
title: Получение workbookPivotTable
description: Получение свойств и связей объекта workbookPivotTable.
ms.openlocfilehash: 5853d7316f7953660064ee24cc9e927bd16a465e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076095"
---
# <a name="get-workbookpivottable"></a><span data-ttu-id="d2da4-103">Получение workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="d2da4-103">Get workbookPivotTable</span></span>

> <span data-ttu-id="d2da4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2da4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2da4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2da4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2da4-106">Получение свойств и связей объекта workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="d2da4-106">Retrieve the properties and relationships of workbookPivotTable object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2da4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2da4-107">Permissions</span></span>
<span data-ttu-id="d2da4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2da4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2da4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2da4-110">Permission type</span></span>      | <span data-ttu-id="d2da4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2da4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2da4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2da4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2da4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2da4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2da4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2da4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2da4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2da4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2da4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2da4-116">Application</span></span> | <span data-ttu-id="d2da4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2da4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2da4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2da4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2da4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2da4-119">Optional query parameters</span></span>
<span data-ttu-id="d2da4-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2da4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2da4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2da4-121">Request headers</span></span>
| <span data-ttu-id="d2da4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d2da4-122">Name</span></span>      |<span data-ttu-id="d2da4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d2da4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2da4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2da4-124">Authorization</span></span>  | <span data-ttu-id="d2da4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2da4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2da4-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2da4-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2da4-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d2da4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2da4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2da4-130">Request body</span></span>
<span data-ttu-id="d2da4-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2da4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2da4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2da4-132">Response</span></span>

<span data-ttu-id="d2da4-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookPivotTable](../resources/workbookpivottable.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2da4-133">If successful, this method returns a `200 OK` response code and [workbookPivotTable](../resources/workbookpivottable.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2da4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d2da4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2da4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2da4-135">Request</span></span>
<span data-ttu-id="d2da4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2da4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}
```
##### <a name="response"></a><span data-ttu-id="d2da4-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2da4-137">Response</span></span>
<span data-ttu-id="d2da4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d2da4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
