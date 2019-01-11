---
title: 'TableRow: delete'
description: Удаляет строку из таблицы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: cea9f8a0801fed24f8767c6929573c729db82d17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861434"
---
# <a name="tablerow-delete"></a><span data-ttu-id="d9449-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="d9449-103">TableRow: delete</span></span>

> <span data-ttu-id="d9449-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d9449-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9449-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9449-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9449-106">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="d9449-106">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9449-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9449-107">Permissions</span></span>
<span data-ttu-id="d9449-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9449-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9449-110">Permission type</span></span>      | <span data-ttu-id="d9449-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9449-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9449-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9449-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d9449-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9449-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9449-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9449-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9449-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9449-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d9449-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9449-116">Application</span></span> | <span data-ttu-id="d9449-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9449-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9449-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9449-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="d9449-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9449-119">Request headers</span></span>
| <span data-ttu-id="d9449-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d9449-120">Name</span></span>       | <span data-ttu-id="d9449-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d9449-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d9449-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9449-122">Authorization</span></span>  | <span data-ttu-id="d9449-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9449-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d9449-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d9449-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d9449-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d9449-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9449-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9449-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d9449-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9449-129">Response</span></span>

<span data-ttu-id="d9449-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d9449-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9449-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d9449-132">Example</span></span>
<span data-ttu-id="d9449-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d9449-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d9449-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9449-134">Request</span></span>
<span data-ttu-id="d9449-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9449-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="d9449-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d9449-136">Response</span></span>
<span data-ttu-id="d9449-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9449-137">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
