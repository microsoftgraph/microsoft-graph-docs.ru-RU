---
title: Обновление таблицы
description: Обновление свойств объекта таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2b78603a261145e2047b5e16175143a3b3c591e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529063"
---
# <a name="update-table"></a><span data-ttu-id="781b7-103">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="781b7-103">Update table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="781b7-104">Обновление свойств объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="781b7-104">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="781b7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="781b7-105">Permissions</span></span>
<span data-ttu-id="781b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="781b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="781b7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="781b7-108">Permission type</span></span>      | <span data-ttu-id="781b7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="781b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="781b7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="781b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="781b7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781b7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="781b7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="781b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="781b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="781b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="781b7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="781b7-114">Application</span></span> | <span data-ttu-id="781b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="781b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="781b7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="781b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="781b7-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="781b7-117">Optional request headers</span></span>
| <span data-ttu-id="781b7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="781b7-118">Name</span></span>       | <span data-ttu-id="781b7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="781b7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="781b7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="781b7-120">Authorization</span></span>  | <span data-ttu-id="781b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="781b7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="781b7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="781b7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="781b7-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="781b7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="781b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="781b7-126">Request body</span></span>
<span data-ttu-id="781b7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="781b7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="781b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="781b7-130">Property</span></span>     | <span data-ttu-id="781b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="781b7-131">Type</span></span>   |<span data-ttu-id="781b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="781b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="781b7-133">name</span><span class="sxs-lookup"><span data-stu-id="781b7-133">name</span></span>|<span data-ttu-id="781b7-134">string</span><span class="sxs-lookup"><span data-stu-id="781b7-134">string</span></span>|<span data-ttu-id="781b7-135">Имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="781b7-135">Name of the table.</span></span>|
|<span data-ttu-id="781b7-136">showHeaders</span><span class="sxs-lookup"><span data-stu-id="781b7-136">showHeaders</span></span>|<span data-ttu-id="781b7-137">boolean</span><span class="sxs-lookup"><span data-stu-id="781b7-137">boolean</span></span>|<span data-ttu-id="781b7-p105">Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.</span><span class="sxs-lookup"><span data-stu-id="781b7-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="781b7-140">showTotals</span><span class="sxs-lookup"><span data-stu-id="781b7-140">showTotals</span></span>|<span data-ttu-id="781b7-141">boolean</span><span class="sxs-lookup"><span data-stu-id="781b7-141">boolean</span></span>|<span data-ttu-id="781b7-p106">Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.</span><span class="sxs-lookup"><span data-stu-id="781b7-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="781b7-144">style</span><span class="sxs-lookup"><span data-stu-id="781b7-144">style</span></span>|<span data-ttu-id="781b7-145">строка</span><span class="sxs-lookup"><span data-stu-id="781b7-145">string</span></span>|<span data-ttu-id="781b7-p107">Постоянное значение, представляющее стиль таблицы. Возможные значения: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Также можно указать настраиваемый пользовательский стиль, имеющийся в книге.</span><span class="sxs-lookup"><span data-stu-id="781b7-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="781b7-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="781b7-149">Response</span></span>

<span data-ttu-id="781b7-150">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Table](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="781b7-150">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="781b7-151">Пример</span><span class="sxs-lookup"><span data-stu-id="781b7-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="781b7-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="781b7-152">Request</span></span>
<span data-ttu-id="781b7-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="781b7-153">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="781b7-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="781b7-154">Response</span></span>
<span data-ttu-id="781b7-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="781b7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
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
<!--
{
  "type": "#page.annotation",
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
