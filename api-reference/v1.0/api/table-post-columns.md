---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 17c49101decad6ad840ff8c564e204ccd6399072
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520643"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="d533f-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="d533f-103">Create TableColumn</span></span>

<span data-ttu-id="d533f-104">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="d533f-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="d533f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d533f-105">Permissions</span></span>
<span data-ttu-id="d533f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d533f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d533f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d533f-108">Permission type</span></span>      | <span data-ttu-id="d533f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d533f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d533f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d533f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d533f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d533f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d533f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d533f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d533f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d533f-113">Not supported.</span></span>    |
|<span data-ttu-id="d533f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d533f-114">Application</span></span> | <span data-ttu-id="d533f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d533f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d533f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d533f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="d533f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d533f-117">Request headers</span></span>
| <span data-ttu-id="d533f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d533f-118">Name</span></span>       | <span data-ttu-id="d533f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d533f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d533f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d533f-120">Authorization</span></span>  | <span data-ttu-id="d533f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d533f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d533f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d533f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d533f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d533f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d533f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d533f-126">Request body</span></span>
<span data-ttu-id="d533f-127">В тексте запроса добавьте представление объекта [Воркбуктаблеколумн](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d533f-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d533f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d533f-128">Response</span></span>

<span data-ttu-id="d533f-129">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [воркбуктаблеколумн](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d533f-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d533f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d533f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d533f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d533f-131">Request</span></span>
<span data-ttu-id="d533f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d533f-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="d533f-133">В тексте запроса добавьте представление объекта [Воркбуктаблеколумн](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d533f-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d533f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d533f-134">Response</span></span>
<span data-ttu-id="d533f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d533f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
