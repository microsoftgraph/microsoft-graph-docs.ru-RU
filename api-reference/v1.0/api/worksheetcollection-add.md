---
title: 'WorksheetCollection: add'
description: .Activate() над ним.
ms.openlocfilehash: 992524aae6dfca0619c043eb0ddb7a4100f50206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025997"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="d6903-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="d6903-103">WorksheetCollection: add</span></span>

<span data-ttu-id="d6903-p101">Добавляет новый лист в книгу. Лист будет добавлен в конец набора имеющихся листов. Если вы хотите активировать только что добавленный лист, вызовите команду .activate().</span><span class="sxs-lookup"><span data-stu-id="d6903-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6903-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6903-107">Permissions</span></span>
<span data-ttu-id="d6903-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6903-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6903-110">Permission type</span></span>      | <span data-ttu-id="d6903-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6903-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6903-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6903-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d6903-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6903-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d6903-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6903-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6903-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6903-115">Not supported.</span></span>    |
|<span data-ttu-id="d6903-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6903-116">Application</span></span> | <span data-ttu-id="d6903-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6903-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6903-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6903-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="d6903-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6903-119">Request headers</span></span>
| <span data-ttu-id="d6903-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d6903-120">Name</span></span>       | <span data-ttu-id="d6903-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d6903-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d6903-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6903-122">Authorization</span></span>  | <span data-ttu-id="d6903-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6903-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d6903-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d6903-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d6903-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d6903-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6903-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6903-128">Request body</span></span>
<span data-ttu-id="d6903-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d6903-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d6903-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d6903-130">Parameter</span></span>    | <span data-ttu-id="d6903-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6903-131">Type</span></span>   |<span data-ttu-id="d6903-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6903-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6903-133">name</span><span class="sxs-lookup"><span data-stu-id="d6903-133">name</span></span>|<span data-ttu-id="d6903-134">строка</span><span class="sxs-lookup"><span data-stu-id="d6903-134">string</span></span>|<span data-ttu-id="d6903-p105">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="d6903-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="d6903-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6903-139">Response</span></span>

<span data-ttu-id="d6903-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [WorkbookWorksheet](../resources/worksheet.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d6903-140">If successful, this method returns `200 OK` response code and [WorkbookWorksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6903-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d6903-141">Example</span></span>
<span data-ttu-id="d6903-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d6903-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d6903-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6903-143">Request</span></span>
<span data-ttu-id="d6903-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6903-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="d6903-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6903-145">Response</span></span>
<span data-ttu-id="d6903-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d6903-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->