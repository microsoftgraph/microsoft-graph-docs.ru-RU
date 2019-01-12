---
title: 'Range: EntireColumn'
description: Возвращает объект, представляющий весь столбец диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2c7dccc535f552edd9f5c6a3d86125471dc78031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925121"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="e780c-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="e780c-103">Range: EntireColumn</span></span>

> <span data-ttu-id="e780c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e780c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e780c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e780c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e780c-106">Возвращает объект, представляющий весь столбец диапазона.</span><span class="sxs-lookup"><span data-stu-id="e780c-106">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="e780c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e780c-107">Permissions</span></span>
<span data-ttu-id="e780c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e780c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e780c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e780c-110">Permission type</span></span>      | <span data-ttu-id="e780c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e780c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e780c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e780c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e780c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e780c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e780c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e780c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e780c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e780c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e780c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e780c-116">Application</span></span> | <span data-ttu-id="e780c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e780c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e780c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e780c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/EntireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/EntireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/EntireColumn

```
## <a name="request-headers"></a><span data-ttu-id="e780c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e780c-119">Request headers</span></span>
| <span data-ttu-id="e780c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e780c-120">Name</span></span>       | <span data-ttu-id="e780c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e780c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e780c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e780c-122">Authorization</span></span>  | <span data-ttu-id="e780c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e780c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e780c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e780c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e780c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e780c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e780c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e780c-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e780c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e780c-129">Response</span></span>

<span data-ttu-id="e780c-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e780c-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e780c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e780c-131">Example</span></span>
<span data-ttu-id="e780c-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e780c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e780c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e780c-133">Request</span></span>
<span data-ttu-id="e780c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e780c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_entirecolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/EntireColumn
```

##### <a name="response"></a><span data-ttu-id="e780c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e780c-135">Response</span></span>
<span data-ttu-id="e780c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e780c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
