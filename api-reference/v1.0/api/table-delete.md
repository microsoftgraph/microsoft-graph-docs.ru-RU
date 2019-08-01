---
title: 'Table: delete'
description: Удаляет таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f4697490d62fd1e39b2e9297d1d2baa24f2d7b8c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024548"
---
# <a name="table-delete"></a><span data-ttu-id="74b02-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="74b02-103">Table: delete</span></span>

<span data-ttu-id="74b02-104">Удаляет таблицу.</span><span class="sxs-lookup"><span data-stu-id="74b02-104">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="74b02-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74b02-105">Permissions</span></span>
<span data-ttu-id="74b02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74b02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74b02-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74b02-108">Permission type</span></span>      | <span data-ttu-id="74b02-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74b02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74b02-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74b02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74b02-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74b02-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74b02-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74b02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74b02-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b02-113">Not supported.</span></span>    |
|<span data-ttu-id="74b02-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74b02-114">Application</span></span> | <span data-ttu-id="74b02-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b02-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74b02-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74b02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="74b02-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74b02-117">Request headers</span></span>
| <span data-ttu-id="74b02-118">Имя</span><span class="sxs-lookup"><span data-stu-id="74b02-118">Name</span></span>       | <span data-ttu-id="74b02-119">Описание</span><span class="sxs-lookup"><span data-stu-id="74b02-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74b02-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74b02-120">Authorization</span></span>  | <span data-ttu-id="74b02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74b02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74b02-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74b02-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="74b02-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="74b02-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74b02-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74b02-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="74b02-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b02-127">Response</span></span>

<span data-ttu-id="74b02-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="74b02-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74b02-130">Пример</span><span class="sxs-lookup"><span data-stu-id="74b02-130">Example</span></span>
<span data-ttu-id="74b02-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="74b02-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74b02-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="74b02-132">Request</span></span>
<span data-ttu-id="74b02-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74b02-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="74b02-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b02-134">Response</span></span>
<span data-ttu-id="74b02-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="74b02-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
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
