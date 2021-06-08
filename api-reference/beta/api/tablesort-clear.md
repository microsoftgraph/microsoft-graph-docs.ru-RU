---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 42577eef5fad03b74175f860cb9ea7b6a997d942
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786876"
---
# <a name="tablesort-clear"></a><span data-ttu-id="d1ca9-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="d1ca9-104">TableSort: clear</span></span>

<span data-ttu-id="d1ca9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1ca9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1ca9-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1ca9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ca9-108">Permissions</span></span>
<span data-ttu-id="d1ca9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1ca9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ca9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1ca9-111">Permission type</span></span>      | <span data-ttu-id="d1ca9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1ca9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1ca9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1ca9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d1ca9-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1ca9-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1ca9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1ca9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1ca9-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1ca9-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d1ca9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1ca9-117">Application</span></span> | <span data-ttu-id="d1ca9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1ca9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1ca9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="d1ca9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1ca9-120">Request headers</span></span>
| <span data-ttu-id="d1ca9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d1ca9-121">Name</span></span>       | <span data-ttu-id="d1ca9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d1ca9-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1ca9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1ca9-123">Authorization</span></span>  | <span data-ttu-id="d1ca9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d1ca9-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d1ca9-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d1ca9-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1ca9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1ca9-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d1ca9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ca9-130">Response</span></span>

<span data-ttu-id="d1ca9-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ca9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d1ca9-133">Example</span></span>
<span data-ttu-id="d1ca9-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d1ca9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1ca9-135">Request</span></span>
<span data-ttu-id="d1ca9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1ca9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1ca9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="d1ca9-138">C#</span><span class="sxs-lookup"><span data-stu-id="d1ca9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1ca9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1ca9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1ca9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1ca9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1ca9-141">Java</span><span class="sxs-lookup"><span data-stu-id="d1ca9-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d1ca9-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1ca9-142">Response</span></span>
<span data-ttu-id="d1ca9-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1ca9-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

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
  ]
}
-->


