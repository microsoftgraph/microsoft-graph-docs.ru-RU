---
title: 'Table: TotalRowRange'
description: Получает объект диапазона, связанный со строкой итогов таблицы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: dab971a08bbf50687c557e7c91ff4dd9753425ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826504"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="538c2-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="538c2-103">Table: TotalRowRange</span></span>

<span data-ttu-id="538c2-104">Получает объект диапазона, связанный со строкой итогов таблицы.</span><span class="sxs-lookup"><span data-stu-id="538c2-104">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="538c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="538c2-105">Permissions</span></span>
<span data-ttu-id="538c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="538c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="538c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="538c2-108">Permission type</span></span>      | <span data-ttu-id="538c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="538c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="538c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="538c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="538c2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="538c2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="538c2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="538c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="538c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="538c2-113">Not supported.</span></span>    |
|<span data-ttu-id="538c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="538c2-114">Application</span></span> | <span data-ttu-id="538c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="538c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="538c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="538c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/totalRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/totalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="538c2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="538c2-117">Request headers</span></span>
| <span data-ttu-id="538c2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="538c2-118">Name</span></span>       | <span data-ttu-id="538c2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="538c2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="538c2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="538c2-120">Authorization</span></span>  | <span data-ttu-id="538c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="538c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="538c2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="538c2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="538c2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="538c2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="538c2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="538c2-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="538c2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="538c2-127">Response</span></span>

<span data-ttu-id="538c2-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="538c2-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538c2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="538c2-129">Example</span></span>
<span data-ttu-id="538c2-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="538c2-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="538c2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="538c2-131">Request</span></span>
<span data-ttu-id="538c2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="538c2-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_totalrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange
```

##### <a name="response"></a><span data-ttu-id="538c2-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="538c2-133">Response</span></span>
<span data-ttu-id="538c2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="538c2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
