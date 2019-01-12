---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 17c49101decad6ad840ff8c564e204ccd6399072
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981226"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="8847b-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="8847b-103">Create TableColumn</span></span>

<span data-ttu-id="8847b-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="8847b-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="8847b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8847b-105">Permissions</span></span>
<span data-ttu-id="8847b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8847b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8847b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8847b-108">Permission type</span></span>      | <span data-ttu-id="8847b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8847b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8847b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8847b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8847b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8847b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8847b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8847b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8847b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8847b-113">Not supported.</span></span>    |
|<span data-ttu-id="8847b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8847b-114">Application</span></span> | <span data-ttu-id="8847b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8847b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8847b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8847b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="8847b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8847b-117">Request headers</span></span>
| <span data-ttu-id="8847b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8847b-118">Name</span></span>       | <span data-ttu-id="8847b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8847b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8847b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8847b-120">Authorization</span></span>  | <span data-ttu-id="8847b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8847b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8847b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8847b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8847b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="8847b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8847b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8847b-126">Request body</span></span>
<span data-ttu-id="8847b-127">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="8847b-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8847b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8847b-128">Response</span></span>

<span data-ttu-id="8847b-129">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [WorkbookTableColumn](../resources/tablecolumn.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8847b-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8847b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8847b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8847b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8847b-131">Request</span></span>
<span data-ttu-id="8847b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8847b-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="8847b-133">В тексте запроса укажите представление JSON объекта [WorkbookTableColumn](../resources/tablecolumn.md) .</span><span class="sxs-lookup"><span data-stu-id="8847b-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8847b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="8847b-134">Response</span></span>
<span data-ttu-id="8847b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8847b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
