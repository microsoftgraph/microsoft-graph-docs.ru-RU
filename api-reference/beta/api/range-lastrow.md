---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1a3f90c4962c2df11f959c23fccebb2fab289f90
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931429"
---
# <a name="range-lastrow"></a><span data-ttu-id="0c4f0-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="0c4f0-103">Range: LastRow</span></span>

> <span data-ttu-id="0c4f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c4f0-p102">Возвращает последнюю строку в диапазоне. Например, последняя строка в диапазоне "B2:D5" — "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="0c4f0-p102">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="0c4f0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4f0-108">Permissions</span></span>
<span data-ttu-id="0c4f0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c4f0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c4f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c4f0-111">Permission type</span></span>      | <span data-ttu-id="0c4f0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c4f0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c4f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c4f0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0c4f0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c4f0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c4f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c4f0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c4f0-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c4f0-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0c4f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c4f0-117">Application</span></span> | <span data-ttu-id="0c4f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c4f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c4f0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="0c4f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c4f0-120">Request headers</span></span>
| <span data-ttu-id="0c4f0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0c4f0-121">Name</span></span>       | <span data-ttu-id="0c4f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0c4f0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c4f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c4f0-123">Authorization</span></span>  | <span data-ttu-id="0c4f0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c4f0-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0c4f0-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="0c4f0-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c4f0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c4f0-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0c4f0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c4f0-130">Response</span></span>

<span data-ttu-id="0c4f0-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-131">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c4f0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0c4f0-132">Example</span></span>
<span data-ttu-id="0c4f0-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c4f0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c4f0-134">Request</span></span>
<span data-ttu-id="0c4f0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="0c4f0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c4f0-136">Response</span></span>
<span data-ttu-id="0c4f0-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0c4f0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
