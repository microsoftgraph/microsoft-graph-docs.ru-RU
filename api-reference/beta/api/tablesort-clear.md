---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: cf0312c35d9042d3bde2d98af10e916aba6de702
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637648"
---
# <a name="tablesort-clear"></a><span data-ttu-id="41c54-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="41c54-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41c54-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="41c54-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="41c54-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41c54-107">Permissions</span></span>
<span data-ttu-id="41c54-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41c54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41c54-110">Permission type</span></span>      | <span data-ttu-id="41c54-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41c54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41c54-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41c54-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41c54-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41c54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41c54-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41c54-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41c54-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41c54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41c54-116">Application</span></span> | <span data-ttu-id="41c54-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41c54-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41c54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41c54-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="41c54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41c54-119">Request headers</span></span>
| <span data-ttu-id="41c54-120">Имя</span><span class="sxs-lookup"><span data-stu-id="41c54-120">Name</span></span>       | <span data-ttu-id="41c54-121">Описание</span><span class="sxs-lookup"><span data-stu-id="41c54-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="41c54-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41c54-122">Authorization</span></span>  | <span data-ttu-id="41c54-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41c54-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41c54-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="41c54-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="41c54-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="41c54-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41c54-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41c54-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="41c54-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="41c54-129">Response</span></span>

<span data-ttu-id="41c54-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="41c54-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41c54-132">Пример</span><span class="sxs-lookup"><span data-stu-id="41c54-132">Example</span></span>
<span data-ttu-id="41c54-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="41c54-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="41c54-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="41c54-134">Request</span></span>
<span data-ttu-id="41c54-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41c54-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="41c54-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="41c54-136">Response</span></span>
<span data-ttu-id="41c54-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41c54-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41c54-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="41c54-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41c54-139">Языках</span><span class="sxs-lookup"><span data-stu-id="41c54-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablesort_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c54-140">Язык</span><span class="sxs-lookup"><span data-stu-id="41c54-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablesort_clear-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
