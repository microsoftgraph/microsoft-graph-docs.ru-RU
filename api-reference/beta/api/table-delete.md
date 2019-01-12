---
title: 'Table: delete'
description: Удаляет таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7896c5c5abd645f71e90ce30d48ffdabefd695c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955767"
---
# <a name="table-delete"></a><span data-ttu-id="d246d-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="d246d-103">Table: delete</span></span>

> <span data-ttu-id="d246d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d246d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d246d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d246d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d246d-106">Удаляет таблицу.</span><span class="sxs-lookup"><span data-stu-id="d246d-106">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d246d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d246d-107">Permissions</span></span>
<span data-ttu-id="d246d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d246d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d246d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d246d-110">Permission type</span></span>      | <span data-ttu-id="d246d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d246d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d246d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d246d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d246d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d246d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d246d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d246d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d246d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d246d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d246d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d246d-116">Application</span></span> | <span data-ttu-id="d246d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d246d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d246d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d246d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="d246d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d246d-119">Request headers</span></span>
| <span data-ttu-id="d246d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d246d-120">Name</span></span>       | <span data-ttu-id="d246d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d246d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d246d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d246d-122">Authorization</span></span>  | <span data-ttu-id="d246d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d246d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d246d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d246d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d246d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d246d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d246d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d246d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d246d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d246d-129">Response</span></span>

<span data-ttu-id="d246d-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d246d-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d246d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d246d-132">Example</span></span>
<span data-ttu-id="d246d-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d246d-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d246d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d246d-134">Request</span></span>
<span data-ttu-id="d246d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d246d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="d246d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d246d-136">Response</span></span>
<span data-ttu-id="d246d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d246d-137">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
