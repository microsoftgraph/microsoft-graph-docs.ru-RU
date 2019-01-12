---
title: 'Range: delete'
description: Удаляет ячейки, связанные с диапазоном.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2a3ea63884964f1c1eb2b423c459fcae3ba6bfb1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931344"
---
# <a name="range-delete"></a><span data-ttu-id="6adec-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="6adec-103">Range: delete</span></span>

> <span data-ttu-id="6adec-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6adec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6adec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6adec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6adec-106">Удаляет ячейки, связанные с диапазоном.</span><span class="sxs-lookup"><span data-stu-id="6adec-106">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="6adec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6adec-107">Permissions</span></span>
<span data-ttu-id="6adec-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6adec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6adec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6adec-110">Permission type</span></span>      | <span data-ttu-id="6adec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6adec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6adec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6adec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6adec-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6adec-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6adec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6adec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6adec-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6adec-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6adec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6adec-116">Application</span></span> | <span data-ttu-id="6adec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6adec-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6adec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6adec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="6adec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6adec-119">Request headers</span></span>
| <span data-ttu-id="6adec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6adec-120">Name</span></span>       | <span data-ttu-id="6adec-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6adec-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6adec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6adec-122">Authorization</span></span>  | <span data-ttu-id="6adec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6adec-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6adec-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6adec-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6adec-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6adec-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6adec-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6adec-128">Request body</span></span>
<span data-ttu-id="6adec-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6adec-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6adec-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="6adec-130">Parameter</span></span>    | <span data-ttu-id="6adec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6adec-131">Type</span></span>   |<span data-ttu-id="6adec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6adec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6adec-133">shift</span><span class="sxs-lookup"><span data-stu-id="6adec-133">shift</span></span>|<span data-ttu-id="6adec-134">строка</span><span class="sxs-lookup"><span data-stu-id="6adec-134">string</span></span>|<span data-ttu-id="6adec-p105">Указывает направление сдвига ячеек.  Возможные значения: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="6adec-p105">Specifies which way to shift the cells.  Possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="6adec-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6adec-137">Response</span></span>

<span data-ttu-id="6adec-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6adec-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6adec-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6adec-140">Example</span></span>
<span data-ttu-id="6adec-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6adec-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6adec-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6adec-142">Request</span></span>
<span data-ttu-id="6adec-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6adec-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6adec-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6adec-144">Response</span></span>
<span data-ttu-id="6adec-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6adec-145">Here is an example of the response.</span></span> 
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
