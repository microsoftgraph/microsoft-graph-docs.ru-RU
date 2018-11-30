---
title: Создание таблицы
description: С помощью этого API можно создать объект Table.
ms.openlocfilehash: a56091ca2ed5e3bad69b3d618fe760db5b350c9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079413"
---
# <a name="create-table"></a><span data-ttu-id="ca124-103">Создание таблицы</span><span class="sxs-lookup"><span data-stu-id="ca124-103">Create table</span></span>

> <span data-ttu-id="ca124-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca124-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca124-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca124-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca124-106">С помощью этого API можно создать объект Table.</span><span class="sxs-lookup"><span data-stu-id="ca124-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca124-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca124-107">Permissions</span></span>
<span data-ttu-id="ca124-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca124-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca124-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca124-110">Permission type</span></span>      | <span data-ttu-id="ca124-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca124-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca124-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca124-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca124-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca124-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca124-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca124-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca124-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca124-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ca124-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca124-116">Application</span></span> | <span data-ttu-id="ca124-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca124-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca124-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca124-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="ca124-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca124-119">Request headers</span></span>
| <span data-ttu-id="ca124-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ca124-120">Name</span></span>       | <span data-ttu-id="ca124-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ca124-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca124-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca124-122">Authorization</span></span>  | <span data-ttu-id="ca124-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca124-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca124-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ca124-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ca124-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ca124-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca124-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca124-128">Request body</span></span>
<span data-ttu-id="ca124-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ca124-129">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="ca124-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca124-130">Parameter</span></span>       | <span data-ttu-id="ca124-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca124-131">Type</span></span>|<span data-ttu-id="ca124-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca124-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="ca124-133">Адрес</span><span class="sxs-lookup"><span data-stu-id="ca124-133">Address</span></span>  | <span data-ttu-id="ca124-134">string</span><span class="sxs-lookup"><span data-stu-id="ca124-134">string</span></span>| <span data-ttu-id="ca124-p105">Адрес диапазона. Если вы отзываете этот API для пути \`worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="ca124-p105">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="ca124-137">Имя} / таблиц и добавления` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `книг и таблиц/добавления` path, then supply the sheet name on which the table needs to be created (example: `sheet1! A1:D4 ")</span><span class="sxs-lookup"><span data-stu-id="ca124-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="ca124-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="ca124-138">hasHeaders</span></span>  | <span data-ttu-id="ca124-139">boolean</span><span class="sxs-lookup"><span data-stu-id="ca124-139">boolean</span></span>|<span data-ttu-id="ca124-p106">Логическое значение, указывающее, имеет ли диапазон метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="ca124-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="ca124-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca124-143">Response</span></span>

<span data-ttu-id="ca124-144">В случае успеха этот метод возвращает код ответа `201 Created` и объект [Table](../resources/table.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca124-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca124-145">Пример</span><span class="sxs-lookup"><span data-stu-id="ca124-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca124-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca124-146">Request</span></span>
<span data-ttu-id="ca124-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca124-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="ca124-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca124-148">Response</span></span>
<span data-ttu-id="ca124-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ca124-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
