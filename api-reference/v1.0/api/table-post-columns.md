---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
ms.openlocfilehash: 00cef446f6f7c75961bb081975af8f908bacc674
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339972"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="2d8eb-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="2d8eb-103">Create TableColumn</span></span>

<span data-ttu-id="2d8eb-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d8eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8eb-105">Permissions</span></span>
<span data-ttu-id="2d8eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d8eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8eb-108">Permission type</span></span>      | <span data-ttu-id="2d8eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d8eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d8eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d8eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d8eb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8eb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d8eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d8eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d8eb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-113">Not supported.</span></span>    |
|<span data-ttu-id="2d8eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d8eb-114">Application</span></span> | <span data-ttu-id="2d8eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d8eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d8eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="2d8eb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d8eb-117">Request headers</span></span>
| <span data-ttu-id="2d8eb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2d8eb-118">Name</span></span>       | <span data-ttu-id="2d8eb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8eb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d8eb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d8eb-120">Authorization</span></span>  | <span data-ttu-id="2d8eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d8eb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2d8eb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2d8eb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d8eb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d8eb-126">Request body</span></span>
<span data-ttu-id="2d8eb-127">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="2d8eb-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2d8eb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d8eb-128">Response</span></span>

<span data-ttu-id="2d8eb-129">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [WorkbookTableColumn](../resources/tablecolumn.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d8eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d8eb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d8eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d8eb-131">Request</span></span>
<span data-ttu-id="2d8eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="2d8eb-133">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="2d8eb-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2d8eb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d8eb-134">Response</span></span>
<span data-ttu-id="2d8eb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2d8eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->