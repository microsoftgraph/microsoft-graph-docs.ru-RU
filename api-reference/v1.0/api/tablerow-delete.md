---
title: 'TableRow: delete'
description: Удаляет строку из таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c98aa15c2e969d760a266842fe03d4a679757dc2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516551"
---
# <a name="tablerow-delete"></a><span data-ttu-id="3e4aa-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="3e4aa-103">TableRow: delete</span></span>

<span data-ttu-id="3e4aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e4aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e4aa-105">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-105">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e4aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4aa-106">Permissions</span></span>
<span data-ttu-id="3e4aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e4aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e4aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e4aa-109">Permission type</span></span>      | <span data-ttu-id="3e4aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e4aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e4aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e4aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e4aa-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e4aa-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e4aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e4aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e4aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-114">Not supported.</span></span>    |
|<span data-ttu-id="3e4aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e4aa-115">Application</span></span> | <span data-ttu-id="3e4aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e4aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e4aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/tables/{id|name}/rows/{index}
DELETE /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}

```
## <a name="request-headers"></a><span data-ttu-id="3e4aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e4aa-118">Request headers</span></span>
| <span data-ttu-id="3e4aa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3e4aa-119">Name</span></span>       | <span data-ttu-id="3e4aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4aa-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e4aa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e4aa-121">Authorization</span></span>  | <span data-ttu-id="3e4aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e4aa-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e4aa-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e4aa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4aa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e4aa-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3e4aa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4aa-128">Response</span></span>

<span data-ttu-id="3e4aa-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4aa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e4aa-131">Example</span></span>
<span data-ttu-id="3e4aa-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e4aa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e4aa-133">Request</span></span>
<span data-ttu-id="3e4aa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}
```

##### <a name="response"></a><span data-ttu-id="3e4aa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e4aa-135">Response</span></span>
<span data-ttu-id="3e4aa-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e4aa-136">Here is an example of the response.</span></span> 
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

