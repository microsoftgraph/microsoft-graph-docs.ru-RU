---
title: 'Table: clearFilters'
description: Удаляет все фильтры, примененные к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 601371e65512bee5ca61641438989f16906500dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967646"
---
# <a name="table-clearfilters"></a><span data-ttu-id="dc14c-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="dc14c-103">Table: clearFilters</span></span>

<span data-ttu-id="dc14c-104">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="dc14c-104">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc14c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc14c-105">Permissions</span></span>
<span data-ttu-id="dc14c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc14c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc14c-108">Permission type</span></span>      | <span data-ttu-id="dc14c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc14c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc14c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc14c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc14c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc14c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dc14c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc14c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc14c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc14c-113">Not supported.</span></span>    |
|<span data-ttu-id="dc14c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc14c-114">Application</span></span> | <span data-ttu-id="dc14c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc14c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc14c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc14c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="dc14c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc14c-117">Request headers</span></span>
| <span data-ttu-id="dc14c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dc14c-118">Name</span></span>       | <span data-ttu-id="dc14c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dc14c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc14c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc14c-120">Authorization</span></span>  | <span data-ttu-id="dc14c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc14c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc14c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dc14c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dc14c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc14c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc14c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc14c-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dc14c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc14c-127">Response</span></span>

<span data-ttu-id="dc14c-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc14c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc14c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dc14c-130">Example</span></span>
<span data-ttu-id="dc14c-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc14c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc14c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc14c-132">Request</span></span>
<span data-ttu-id="dc14c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc14c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="dc14c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc14c-134">Response</span></span>
<span data-ttu-id="dc14c-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc14c-135">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
