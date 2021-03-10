---
title: 'TableColumn: delete'
description: Удаляет столбец из таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2154bbb7a28d34b08ec1e8cbfa0f6ca3fa14f1ef
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578341"
---
# <a name="tablecolumn-delete"></a><span data-ttu-id="5065e-103">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="5065e-103">TableColumn: delete</span></span>

<span data-ttu-id="5065e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5065e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5065e-105">Удаляет столбец из таблицы.</span><span class="sxs-lookup"><span data-stu-id="5065e-105">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="5065e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5065e-106">Permissions</span></span>
<span data-ttu-id="5065e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5065e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5065e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5065e-109">Permission type</span></span>      | <span data-ttu-id="5065e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5065e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5065e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5065e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5065e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5065e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5065e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5065e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5065e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5065e-114">Not supported.</span></span>    |
|<span data-ttu-id="5065e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5065e-115">Application</span></span> | <span data-ttu-id="5065e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5065e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5065e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5065e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="5065e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5065e-118">Request headers</span></span>
| <span data-ttu-id="5065e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5065e-119">Name</span></span>       | <span data-ttu-id="5065e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5065e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5065e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5065e-121">Authorization</span></span>  | <span data-ttu-id="5065e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5065e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5065e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5065e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5065e-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="5065e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5065e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5065e-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5065e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5065e-128">Response</span></span>

<span data-ttu-id="5065e-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5065e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5065e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5065e-131">Example</span></span>
<span data-ttu-id="5065e-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5065e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5065e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5065e-133">Request</span></span>
<span data-ttu-id="5065e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5065e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}
```

##### <a name="response"></a><span data-ttu-id="5065e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5065e-135">Response</span></span>
<span data-ttu-id="5065e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5065e-136">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

