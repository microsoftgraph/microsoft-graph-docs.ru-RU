---
title: Список листов
description: Получение списка объектов листов.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 02d26e4130019e232a23af0eae7ea25678285d3c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575323"
---
# <a name="list-worksheets"></a><span data-ttu-id="f9c96-103">Список листов</span><span class="sxs-lookup"><span data-stu-id="f9c96-103">List worksheets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9c96-104">Получение списка объектов листов.</span><span class="sxs-lookup"><span data-stu-id="f9c96-104">Retrieve a list of worksheet objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9c96-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c96-105">Permissions</span></span>
<span data-ttu-id="f9c96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9c96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c96-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9c96-108">Permission type</span></span>      | <span data-ttu-id="f9c96-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9c96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9c96-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9c96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9c96-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9c96-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9c96-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9c96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9c96-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9c96-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9c96-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9c96-114">Application</span></span> | <span data-ttu-id="f9c96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9c96-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9c96-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9c96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9c96-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9c96-117">Optional query parameters</span></span>
<span data-ttu-id="f9c96-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9c96-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9c96-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9c96-119">Request headers</span></span>
| <span data-ttu-id="f9c96-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f9c96-120">Name</span></span>      |<span data-ttu-id="f9c96-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f9c96-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9c96-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9c96-122">Authorization</span></span>  | <span data-ttu-id="f9c96-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9c96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9c96-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9c96-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9c96-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f9c96-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c96-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9c96-128">Request body</span></span>
<span data-ttu-id="f9c96-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9c96-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9c96-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c96-130">Response</span></span>

<span data-ttu-id="f9c96-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9c96-131">If successful, this method returns a `200 OK` response code and collection of [Worksheet](../resources/worksheet.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9c96-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f9c96-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9c96-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9c96-133">Request</span></span>
<span data-ttu-id="f9c96-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9c96-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_worksheets"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets
```
##### <a name="response"></a><span data-ttu-id="f9c96-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9c96-135">Response</span></span>
<span data-ttu-id="f9c96-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f9c96-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "id": "id-value",
      "position": 99,
      "name": "name-value",
      "visibility": "visibility-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List worksheets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/workbook-list-worksheets.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
