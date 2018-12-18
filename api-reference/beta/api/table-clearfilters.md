---
title: 'Table: clearFilters'
description: Удаляет все фильтры, примененные к таблице.
author: lumine2008
ms.openlocfilehash: b887cd0732827e19b19d42142c1c00be9a7b2307
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340154"
---
# <a name="table-clearfilters"></a><span data-ttu-id="2dff8-103">Table: clearFilters</span><span class="sxs-lookup"><span data-stu-id="2dff8-103">Table: clearFilters</span></span>

> <span data-ttu-id="2dff8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2dff8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dff8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dff8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2dff8-106">Очищает все фильтры, примененные к таблице.</span><span class="sxs-lookup"><span data-stu-id="2dff8-106">Clears all the filters currently applied on the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2dff8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2dff8-107">Permissions</span></span>
<span data-ttu-id="2dff8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dff8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dff8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dff8-110">Permission type</span></span>      | <span data-ttu-id="2dff8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dff8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dff8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dff8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2dff8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dff8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dff8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dff8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dff8-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dff8-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dff8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dff8-116">Application</span></span> | <span data-ttu-id="2dff8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dff8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dff8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dff8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/clearFilters
POST /workbook/worksheets/{id|name}/tables/{id|name}/clearFilters

```
## <a name="request-headers"></a><span data-ttu-id="2dff8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2dff8-119">Request headers</span></span>
| <span data-ttu-id="2dff8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2dff8-120">Name</span></span>       | <span data-ttu-id="2dff8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2dff8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2dff8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dff8-122">Authorization</span></span>  | <span data-ttu-id="2dff8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dff8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2dff8-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2dff8-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2dff8-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2dff8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dff8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2dff8-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2dff8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2dff8-129">Response</span></span>

<span data-ttu-id="2dff8-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2dff8-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dff8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2dff8-132">Example</span></span>
<span data-ttu-id="2dff8-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2dff8-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2dff8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dff8-134">Request</span></span>
<span data-ttu-id="2dff8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2dff8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_clearfilters"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters
```

##### <a name="response"></a><span data-ttu-id="2dff8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2dff8-136">Response</span></span>
<span data-ttu-id="2dff8-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2dff8-137">Here is an example of the response.</span></span> 
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
  "description": "Table: clearFilters",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->