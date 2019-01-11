---
title: 'TableColumn: HeaderRowRange'
description: Получает объект диапазона, связанный со строкой заголовков столбца.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 85d61fa2bfe8d5b4a625e4e2c53bfb9321ed4b98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841302"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="d346d-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="d346d-103">TableColumn: HeaderRowRange</span></span>

> <span data-ttu-id="d346d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d346d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d346d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d346d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d346d-106">Получает объект диапазона, связанный со строкой заголовков столбца.</span><span class="sxs-lookup"><span data-stu-id="d346d-106">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="d346d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d346d-107">Permissions</span></span>
<span data-ttu-id="d346d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d346d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d346d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d346d-110">Permission type</span></span>      | <span data-ttu-id="d346d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d346d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d346d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d346d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d346d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d346d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d346d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d346d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d346d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d346d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d346d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d346d-116">Application</span></span> | <span data-ttu-id="d346d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d346d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d346d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d346d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="d346d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d346d-119">Request headers</span></span>
| <span data-ttu-id="d346d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d346d-120">Name</span></span>       | <span data-ttu-id="d346d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d346d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d346d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d346d-122">Authorization</span></span>  | <span data-ttu-id="d346d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d346d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d346d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d346d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d346d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d346d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d346d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d346d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d346d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d346d-129">Response</span></span>

<span data-ttu-id="d346d-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d346d-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d346d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d346d-131">Example</span></span>
<span data-ttu-id="d346d-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d346d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d346d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d346d-133">Request</span></span>
<span data-ttu-id="d346d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d346d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="d346d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d346d-135">Response</span></span>
<span data-ttu-id="d346d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d346d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
