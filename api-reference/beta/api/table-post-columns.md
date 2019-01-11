---
title: Создание объекта TableColumn
description: С помощью этого API можно создать объект TableColumn.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8c315cd4de26dd610a99e7df66b67856e17b3fb0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820729"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="96ef7-103">Создание объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="96ef7-103">Create TableColumn</span></span>

> <span data-ttu-id="96ef7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96ef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96ef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96ef7-106">С помощью этого API можно создать объект TableColumn.</span><span class="sxs-lookup"><span data-stu-id="96ef7-106">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="96ef7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96ef7-107">Permissions</span></span>
<span data-ttu-id="96ef7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ef7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ef7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96ef7-110">Permission type</span></span>      | <span data-ttu-id="96ef7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96ef7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96ef7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96ef7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96ef7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96ef7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96ef7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96ef7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96ef7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96ef7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96ef7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96ef7-116">Application</span></span> | <span data-ttu-id="96ef7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ef7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96ef7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96ef7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="96ef7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96ef7-119">Request headers</span></span>
| <span data-ttu-id="96ef7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="96ef7-120">Name</span></span>       | <span data-ttu-id="96ef7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="96ef7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96ef7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96ef7-122">Authorization</span></span>  | <span data-ttu-id="96ef7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96ef7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96ef7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96ef7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="96ef7-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="96ef7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ef7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96ef7-128">Request body</span></span>
<span data-ttu-id="96ef7-129">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96ef7-129">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="96ef7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ef7-130">Response</span></span>

<span data-ttu-id="96ef7-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [TableColumn](../resources/tablecolumn.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96ef7-131">If successful, this method returns `201 Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ef7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="96ef7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96ef7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="96ef7-133">Request</span></span>
<span data-ttu-id="96ef7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96ef7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="96ef7-135">Предоставьте в тексте запроса описание объекта [TableColumn](../resources/tablecolumn.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96ef7-135">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="96ef7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ef7-136">Response</span></span>
<span data-ttu-id="96ef7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96ef7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
