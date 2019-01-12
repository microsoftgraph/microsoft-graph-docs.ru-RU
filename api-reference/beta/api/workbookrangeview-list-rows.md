---
title: Получение списка строк rangeView
description: Получение списка, который включает в себя объекты видимых ячеек в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 60cacae78c8ab2920da8133e5a95773bf21fae66
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923583"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="7ced9-103">Получение списка строк rangeView</span><span class="sxs-lookup"><span data-stu-id="7ced9-103">List rangeView rows</span></span>

> <span data-ttu-id="7ced9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ced9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ced9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ced9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ced9-106">Получение списка, который включает в себя объекты видимых ячеек в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="7ced9-106">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ced9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ced9-107">Permissions</span></span>
<span data-ttu-id="7ced9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ced9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ced9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ced9-110">Permission type</span></span>      | <span data-ttu-id="7ced9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ced9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ced9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ced9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ced9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ced9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ced9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ced9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ced9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ced9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7ced9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ced9-116">Application</span></span> | <span data-ttu-id="7ced9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ced9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ced9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ced9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ced9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ced9-119">Optional query parameters</span></span>
<span data-ttu-id="7ced9-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ced9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ced9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ced9-121">Request headers</span></span>
| <span data-ttu-id="7ced9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7ced9-122">Name</span></span>      |<span data-ttu-id="7ced9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7ced9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ced9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ced9-124">Authorization</span></span>  | <span data-ttu-id="7ced9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ced9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7ced9-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7ced9-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="7ced9-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7ced9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ced9-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ced9-130">Request body</span></span>
<span data-ttu-id="7ced9-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ced9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ced9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ced9-132">Response</span></span>

<span data-ttu-id="7ced9-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ced9-133">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ced9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7ced9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ced9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ced9-135">Request</span></span>
<span data-ttu-id="7ced9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ced9-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="7ced9-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ced9-137">Response</span></span>
<span data-ttu-id="7ced9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ced9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
