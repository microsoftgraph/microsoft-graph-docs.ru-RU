---
title: 'TableColumn: Range'
description: Получает объект диапазона, связанный со всем столбцом.
author: lumine2008
ms.openlocfilehash: ef3615d78ca4c4121d69db68e7cb3cdb6840ad01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328933"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="1b89d-103">TableColumn: Range</span><span class="sxs-lookup"><span data-stu-id="1b89d-103">TableColumn: Range</span></span>

> <span data-ttu-id="1b89d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b89d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b89d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b89d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b89d-106">Получает объект диапазона, связанный со всем столбцом.</span><span class="sxs-lookup"><span data-stu-id="1b89d-106">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b89d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b89d-107">Permissions</span></span>
<span data-ttu-id="1b89d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b89d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b89d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b89d-110">Permission type</span></span>      | <span data-ttu-id="1b89d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b89d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b89d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b89d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b89d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b89d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1b89d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b89d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b89d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b89d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1b89d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b89d-116">Application</span></span> | <span data-ttu-id="1b89d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b89d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b89d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b89d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="1b89d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b89d-119">Request headers</span></span>
| <span data-ttu-id="1b89d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1b89d-120">Name</span></span>       | <span data-ttu-id="1b89d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1b89d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b89d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b89d-122">Authorization</span></span>  | <span data-ttu-id="1b89d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b89d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b89d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1b89d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1b89d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1b89d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b89d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b89d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1b89d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b89d-129">Response</span></span>

<span data-ttu-id="1b89d-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b89d-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b89d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1b89d-131">Example</span></span>
<span data-ttu-id="1b89d-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1b89d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b89d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b89d-133">Request</span></span>
<span data-ttu-id="1b89d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b89d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range
```

##### <a name="response"></a><span data-ttu-id="1b89d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b89d-135">Response</span></span>
<span data-ttu-id="1b89d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b89d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->