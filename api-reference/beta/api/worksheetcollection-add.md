---
title: 'WorksheetCollection: add'
description: .Activate() над ним.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: df5cf2fcdd406802e370fc292480fc012cbc6e8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882763"
---
# <a name="worksheetcollection-add"></a><span data-ttu-id="e7da3-103">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="e7da3-103">WorksheetCollection: add</span></span>

> <span data-ttu-id="e7da3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7da3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7da3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7da3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7da3-p102">Добавляет новый лист в книгу. Лист будет добавлен в конец набора имеющихся листов. Если вы хотите активировать только что добавленный лист, вызовите команду .activate().</span><span class="sxs-lookup"><span data-stu-id="e7da3-p102">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7da3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7da3-109">Permissions</span></span>
<span data-ttu-id="e7da3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7da3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7da3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7da3-112">Permission type</span></span>      | <span data-ttu-id="e7da3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7da3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7da3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7da3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e7da3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7da3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7da3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7da3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7da3-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7da3-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7da3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7da3-118">Application</span></span> | <span data-ttu-id="e7da3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7da3-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7da3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7da3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="e7da3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7da3-121">Request headers</span></span>
| <span data-ttu-id="e7da3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e7da3-122">Name</span></span>       | <span data-ttu-id="e7da3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e7da3-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e7da3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7da3-124">Authorization</span></span>  | <span data-ttu-id="e7da3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7da3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7da3-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7da3-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7da3-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e7da3-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7da3-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7da3-130">Request body</span></span>
<span data-ttu-id="e7da3-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e7da3-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7da3-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="e7da3-132">Parameter</span></span>    | <span data-ttu-id="e7da3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e7da3-133">Type</span></span>   |<span data-ttu-id="e7da3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e7da3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7da3-135">name</span><span class="sxs-lookup"><span data-stu-id="e7da3-135">name</span></span>|<span data-ttu-id="e7da3-136">строка</span><span class="sxs-lookup"><span data-stu-id="e7da3-136">string</span></span>|<span data-ttu-id="e7da3-p106">Необязательный параметр. Имя добавляемого листа. Если параметр используется, имя должно быть уникальным. В противном случае Excel определяет имя нового листа.</span><span class="sxs-lookup"><span data-stu-id="e7da3-p106">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="e7da3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7da3-141">Response</span></span>

<span data-ttu-id="e7da3-142">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Worksheet](../resources/worksheet.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7da3-142">If successful, this method returns `200 OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7da3-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e7da3-143">Example</span></span>
<span data-ttu-id="e7da3-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e7da3-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e7da3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7da3-145">Request</span></span>
<span data-ttu-id="e7da3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7da3-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e7da3-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7da3-147">Response</span></span>
<span data-ttu-id="e7da3-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7da3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
