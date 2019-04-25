---
title: 'Table: reapplyFilters'
description: Повторно применяет все текущие фильтры к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e09541c81b3f9675df67fe484fc79bd43c03f602
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520503"
---
# <a name="table-reapplyfilters"></a><span data-ttu-id="7906f-103">Table: reapplyFilters</span><span class="sxs-lookup"><span data-stu-id="7906f-103">Table: reapplyFilters</span></span>

<span data-ttu-id="7906f-104">Повторно применяет все текущие фильтры к таблице.</span><span class="sxs-lookup"><span data-stu-id="7906f-104">Reapplies all the filters currently on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7906f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7906f-105">Permissions</span></span>
<span data-ttu-id="7906f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7906f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7906f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7906f-108">Permission type</span></span>      | <span data-ttu-id="7906f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7906f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7906f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7906f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7906f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7906f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7906f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7906f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7906f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7906f-113">Not supported.</span></span>    |
|<span data-ttu-id="7906f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7906f-114">Application</span></span> | <span data-ttu-id="7906f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7906f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7906f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7906f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/reapplyFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/reapplyFilters

```
## <a name="request-headers"></a><span data-ttu-id="7906f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7906f-117">Request headers</span></span>
| <span data-ttu-id="7906f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7906f-118">Name</span></span>       | <span data-ttu-id="7906f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7906f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7906f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7906f-120">Authorization</span></span>  | <span data-ttu-id="7906f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7906f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7906f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7906f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7906f-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7906f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7906f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7906f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7906f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7906f-127">Response</span></span>

<span data-ttu-id="7906f-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7906f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7906f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7906f-130">Example</span></span>
<span data-ttu-id="7906f-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7906f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7906f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7906f-132">Request</span></span>
<span data-ttu-id="7906f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7906f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_reapplyfilters"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters
```

##### <a name="response"></a><span data-ttu-id="7906f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7906f-134">Response</span></span>
<span data-ttu-id="7906f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7906f-135">Here is an example of the response.</span></span> 
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
  "description": "Table: reapplyFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
