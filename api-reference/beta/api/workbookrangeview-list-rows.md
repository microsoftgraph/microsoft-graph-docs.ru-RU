---
title: Получение списка строк rangeView
description: Получение списка, который включает в себя объекты видимых ячеек в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9d0d3cb5f29f9588481b5e87c7a20cc96e3850e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523003"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="6eb04-103">Получение списка строк rangeView</span><span class="sxs-lookup"><span data-stu-id="6eb04-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb04-104">Получение списка, который включает в себя объекты видимых ячеек в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="6eb04-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6eb04-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6eb04-105">Permissions</span></span>
<span data-ttu-id="6eb04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eb04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb04-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6eb04-108">Permission type</span></span>      | <span data-ttu-id="6eb04-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6eb04-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6eb04-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6eb04-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6eb04-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6eb04-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6eb04-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6eb04-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6eb04-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6eb04-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6eb04-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6eb04-114">Application</span></span> | <span data-ttu-id="6eb04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eb04-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6eb04-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6eb04-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="6eb04-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6eb04-117">Optional query parameters</span></span>
<span data-ttu-id="6eb04-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6eb04-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6eb04-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6eb04-119">Request headers</span></span>
| <span data-ttu-id="6eb04-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6eb04-120">Name</span></span>      |<span data-ttu-id="6eb04-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb04-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6eb04-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6eb04-122">Authorization</span></span>  | <span data-ttu-id="6eb04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6eb04-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6eb04-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6eb04-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6eb04-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6eb04-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb04-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6eb04-128">Request body</span></span>
<span data-ttu-id="6eb04-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6eb04-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6eb04-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6eb04-130">Response</span></span>

<span data-ttu-id="6eb04-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6eb04-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6eb04-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6eb04-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6eb04-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6eb04-133">Request</span></span>
<span data-ttu-id="6eb04-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6eb04-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="6eb04-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6eb04-135">Response</span></span>
<span data-ttu-id="6eb04-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6eb04-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-list-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
