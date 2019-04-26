---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 59531c4a4d8fa3abcb3a857cbaca4487299b8d6e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337038"
---
# <a name="range-delete"></a><span data-ttu-id="57ee2-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="57ee2-103">Range: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57ee2-104">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="57ee2-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="57ee2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57ee2-105">Permissions</span></span>
<span data-ttu-id="57ee2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ee2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57ee2-108">Permission type</span></span>      | <span data-ttu-id="57ee2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57ee2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57ee2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57ee2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57ee2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57ee2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57ee2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57ee2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57ee2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57ee2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="57ee2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57ee2-114">Application</span></span> | <span data-ttu-id="57ee2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ee2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57ee2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57ee2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="57ee2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57ee2-117">Request headers</span></span>
| <span data-ttu-id="57ee2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="57ee2-118">Name</span></span>       | <span data-ttu-id="57ee2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="57ee2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="57ee2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57ee2-120">Authorization</span></span>  | <span data-ttu-id="57ee2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57ee2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57ee2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="57ee2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="57ee2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="57ee2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ee2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57ee2-126">Request body</span></span>
<span data-ttu-id="57ee2-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="57ee2-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57ee2-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="57ee2-128">Parameter</span></span>    | <span data-ttu-id="57ee2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="57ee2-129">Type</span></span>   |<span data-ttu-id="57ee2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="57ee2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57ee2-131">shift</span><span class="sxs-lookup"><span data-stu-id="57ee2-131">shift</span></span>|<span data-ttu-id="57ee2-132">string</span><span class="sxs-lookup"><span data-stu-id="57ee2-132">string</span></span>|<span data-ttu-id="57ee2-p104">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="57ee2-p104">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="57ee2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ee2-135">Response</span></span>

<span data-ttu-id="57ee2-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="57ee2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57ee2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="57ee2-138">Example</span></span>
<span data-ttu-id="57ee2-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57ee2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="57ee2-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="57ee2-140">Request</span></span>
<span data-ttu-id="57ee2-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57ee2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="57ee2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="57ee2-142">Response</span></span>
<span data-ttu-id="57ee2-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57ee2-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
