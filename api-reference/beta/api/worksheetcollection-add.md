---
title: 'WorksheetCollection: add'
description: .Activate() над ним.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0958f8f82502c92eff08ec80a7b116c1b0c4a5f0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508050"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="485fb-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="485fb-103">WorksheetCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="485fb-p101">Добавляет новый лист в книгу. Лист будет добавлен в конец набора имеющихся листов. Если вы хотите активировать только что добавленный лист, вызовите команду .activate().</span><span class="sxs-lookup"><span data-stu-id="485fb-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="485fb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485fb-107">Permissions</span></span>
<span data-ttu-id="485fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485fb-110">Permission type</span></span>      | <span data-ttu-id="485fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="485fb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485fb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="485fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485fb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485fb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="485fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485fb-116">Application</span></span> | <span data-ttu-id="485fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="485fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="485fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="485fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485fb-119">Request headers</span></span>
| <span data-ttu-id="485fb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="485fb-120">Name</span></span>       | <span data-ttu-id="485fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="485fb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="485fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="485fb-122">Authorization</span></span>  | <span data-ttu-id="485fb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="485fb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="485fb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="485fb-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="485fb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="485fb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="485fb-128">Request body</span></span>
<span data-ttu-id="485fb-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="485fb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="485fb-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="485fb-130">Parameter</span></span>    | <span data-ttu-id="485fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="485fb-131">Type</span></span>   |<span data-ttu-id="485fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="485fb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="485fb-133">name</span><span class="sxs-lookup"><span data-stu-id="485fb-133">name</span></span>|<span data-ttu-id="485fb-134">строка</span><span class="sxs-lookup"><span data-stu-id="485fb-134">string</span></span>|<span data-ttu-id="485fb-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="485fb-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="485fb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="485fb-139">Response</span></span>

<span data-ttu-id="485fb-140">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="485fb-140">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485fb-141">Пример</span><span class="sxs-lookup"><span data-stu-id="485fb-141">Example</span></span>
<span data-ttu-id="485fb-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="485fb-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="485fb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="485fb-143">Request</span></span>
<span data-ttu-id="485fb-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="485fb-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="485fb-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="485fb-145">Response</span></span>
<span data-ttu-id="485fb-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="485fb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheetcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
