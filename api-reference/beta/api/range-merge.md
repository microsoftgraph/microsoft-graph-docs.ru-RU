---
title: 'Range: merge'
description: Объединяет ячейки диапазона в одну область на листе.
author: lumine2008
ms.openlocfilehash: 628acea9c86ff7cf8b460fb5db2abb7157c85146
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317341"
---
# <a name="range-merge"></a><span data-ttu-id="d75a8-103">Range: merge</span><span class="sxs-lookup"><span data-stu-id="d75a8-103">Range: merge</span></span>

> <span data-ttu-id="d75a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d75a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d75a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d75a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d75a8-106">Объединяет ячейки диапазона в одну область на листе.</span><span class="sxs-lookup"><span data-stu-id="d75a8-106">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="d75a8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d75a8-107">Permissions</span></span>
<span data-ttu-id="d75a8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d75a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d75a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d75a8-110">Permission type</span></span>      | <span data-ttu-id="d75a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d75a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d75a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d75a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d75a8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d75a8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d75a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d75a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d75a8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d75a8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d75a8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d75a8-116">Application</span></span> | <span data-ttu-id="d75a8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d75a8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d75a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d75a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="d75a8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d75a8-119">Request headers</span></span>
| <span data-ttu-id="d75a8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d75a8-120">Name</span></span>       | <span data-ttu-id="d75a8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d75a8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d75a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d75a8-122">Authorization</span></span>  | <span data-ttu-id="d75a8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d75a8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d75a8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d75a8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d75a8-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d75a8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d75a8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d75a8-128">Request body</span></span>
<span data-ttu-id="d75a8-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d75a8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d75a8-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d75a8-130">Parameter</span></span>    | <span data-ttu-id="d75a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d75a8-131">Type</span></span>   |<span data-ttu-id="d75a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d75a8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d75a8-133">across</span><span class="sxs-lookup"><span data-stu-id="d75a8-133">across</span></span>|<span data-ttu-id="d75a8-134">boolean</span><span class="sxs-lookup"><span data-stu-id="d75a8-134">boolean</span></span>|<span data-ttu-id="d75a8-p105">Необязательный параметр. Установите значение true, чтобы объединить ячейки в каждой строке заданного диапазона как отдельные объединенные ячейки. Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="d75a8-p105">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="d75a8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d75a8-138">Response</span></span>

<span data-ttu-id="d75a8-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d75a8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d75a8-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d75a8-141">Example</span></span>
<span data-ttu-id="d75a8-142">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d75a8-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d75a8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d75a8-143">Request</span></span>
<span data-ttu-id="d75a8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d75a8-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="d75a8-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="d75a8-145">Response</span></span>
<span data-ttu-id="d75a8-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d75a8-146">Here is an example of the response.</span></span> 
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
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->