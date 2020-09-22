---
title: 'TableRow: delete'
description: Удаляет строку из таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b9e0ddaead438d3df4cc01ecd193f213576569f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012868"
---
# <a name="tablerow-delete"></a><span data-ttu-id="7d0be-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="7d0be-103">TableRow: delete</span></span>

<span data-ttu-id="7d0be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d0be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d0be-105">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="7d0be-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d0be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0be-106">Permissions</span></span>
<span data-ttu-id="7d0be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d0be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d0be-109">Permission type</span></span>      | <span data-ttu-id="7d0be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d0be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d0be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d0be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7d0be-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0be-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7d0be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d0be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d0be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d0be-114">Not supported.</span></span>    |
|<span data-ttu-id="7d0be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d0be-115">Application</span></span> | <span data-ttu-id="7d0be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d0be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d0be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d0be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="7d0be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d0be-118">Request headers</span></span>
| <span data-ttu-id="7d0be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7d0be-119">Name</span></span>       | <span data-ttu-id="7d0be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7d0be-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d0be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d0be-121">Authorization</span></span>  | <span data-ttu-id="7d0be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7d0be-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7d0be-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7d0be-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d0be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d0be-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7d0be-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0be-128">Response</span></span>

<span data-ttu-id="7d0be-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7d0be-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d0be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d0be-131">Example</span></span>
<span data-ttu-id="7d0be-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7d0be-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d0be-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d0be-133">Request</span></span>
<span data-ttu-id="7d0be-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d0be-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="7d0be-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d0be-135">Response</span></span>
<span data-ttu-id="7d0be-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7d0be-136">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

