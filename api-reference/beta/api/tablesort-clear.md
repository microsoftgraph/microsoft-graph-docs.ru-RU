---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3e2e6e30fa0fe457c4ee603d06d02d2f8940e782
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575345"
---
# <a name="tablesort-clear"></a><span data-ttu-id="cd60f-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="cd60f-104">TableSort: clear</span></span>

<span data-ttu-id="cd60f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd60f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd60f-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="cd60f-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd60f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd60f-108">Permissions</span></span>
<span data-ttu-id="cd60f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd60f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd60f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd60f-111">Permission type</span></span>      | <span data-ttu-id="cd60f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd60f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd60f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd60f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cd60f-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd60f-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd60f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd60f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd60f-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd60f-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd60f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd60f-117">Application</span></span> | <span data-ttu-id="cd60f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd60f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd60f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd60f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="cd60f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd60f-120">Request headers</span></span>
| <span data-ttu-id="cd60f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cd60f-121">Name</span></span>       | <span data-ttu-id="cd60f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd60f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd60f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd60f-123">Authorization</span></span>  | <span data-ttu-id="cd60f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd60f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd60f-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd60f-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd60f-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cd60f-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd60f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd60f-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cd60f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd60f-130">Response</span></span>

<span data-ttu-id="cd60f-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cd60f-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd60f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cd60f-133">Example</span></span>
<span data-ttu-id="cd60f-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cd60f-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd60f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd60f-135">Request</span></span>
<span data-ttu-id="cd60f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd60f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd60f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd60f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="cd60f-138">C#</span><span class="sxs-lookup"><span data-stu-id="cd60f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd60f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd60f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd60f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd60f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd60f-141">Java</span><span class="sxs-lookup"><span data-stu-id="cd60f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cd60f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd60f-142">Response</span></span>
<span data-ttu-id="cd60f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd60f-143">Here is an example of the response.</span></span> 
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


