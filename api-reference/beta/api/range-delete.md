---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 1817a1c1481d86e08de4146215da6f6fc8de6a8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871787"
---
# <a name="range-delete"></a><span data-ttu-id="1433f-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="1433f-103">Range: delete</span></span>

> <span data-ttu-id="1433f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1433f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1433f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1433f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1433f-106">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="1433f-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="1433f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1433f-107">Permissions</span></span>
<span data-ttu-id="1433f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1433f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1433f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1433f-110">Permission type</span></span>      | <span data-ttu-id="1433f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1433f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1433f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1433f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1433f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1433f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1433f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1433f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1433f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1433f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1433f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1433f-116">Application</span></span> | <span data-ttu-id="1433f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1433f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1433f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1433f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="1433f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1433f-119">Request headers</span></span>
| <span data-ttu-id="1433f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1433f-120">Name</span></span>       | <span data-ttu-id="1433f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1433f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1433f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1433f-122">Authorization</span></span>  | <span data-ttu-id="1433f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1433f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1433f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1433f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1433f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1433f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1433f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1433f-128">Request body</span></span>
<span data-ttu-id="1433f-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1433f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1433f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="1433f-130">Parameter</span></span>    | <span data-ttu-id="1433f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1433f-131">Type</span></span>   |<span data-ttu-id="1433f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1433f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1433f-133">shift</span><span class="sxs-lookup"><span data-stu-id="1433f-133">shift</span></span>|<span data-ttu-id="1433f-134">string</span><span class="sxs-lookup"><span data-stu-id="1433f-134">string</span></span>|<span data-ttu-id="1433f-p105">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="1433f-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="1433f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1433f-137">Response</span></span>

<span data-ttu-id="1433f-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1433f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1433f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1433f-140">Example</span></span>
<span data-ttu-id="1433f-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1433f-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1433f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1433f-142">Request</span></span>
<span data-ttu-id="1433f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1433f-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="1433f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="1433f-144">Response</span></span>
<span data-ttu-id="1433f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1433f-145">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
