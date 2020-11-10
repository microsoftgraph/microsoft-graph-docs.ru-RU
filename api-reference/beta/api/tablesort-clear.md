---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 224ab0f518a4011014b57d2ede2fb0956b0cdb3d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976431"
---
# <a name="tablesort-clear"></a><span data-ttu-id="ddb1b-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="ddb1b-104">TableSort: clear</span></span>

<span data-ttu-id="ddb1b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb1b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb1b-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="ddb1b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb1b-108">Permissions</span></span>
<span data-ttu-id="ddb1b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb1b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb1b-111">Permission type</span></span>      | <span data-ttu-id="ddb1b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb1b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddb1b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb1b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ddb1b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb1b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddb1b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb1b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb1b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ddb1b-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ddb1b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddb1b-117">Application</span></span> | <span data-ttu-id="ddb1b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb1b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="ddb1b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddb1b-120">Request headers</span></span>
| <span data-ttu-id="ddb1b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ddb1b-121">Name</span></span>       | <span data-ttu-id="ddb1b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb1b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ddb1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb1b-123">Authorization</span></span>  | <span data-ttu-id="ddb1b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddb1b-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ddb1b-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="ddb1b-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb1b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddb1b-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ddb1b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb1b-130">Response</span></span>

<span data-ttu-id="ddb1b-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddb1b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb1b-133">Example</span></span>
<span data-ttu-id="ddb1b-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ddb1b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb1b-135">Request</span></span>
<span data-ttu-id="ddb1b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddb1b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb1b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="ddb1b-138">C#</span><span class="sxs-lookup"><span data-stu-id="ddb1b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddb1b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb1b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddb1b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddb1b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddb1b-141">Java</span><span class="sxs-lookup"><span data-stu-id="ddb1b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ddb1b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb1b-142">Response</span></span>
<span data-ttu-id="ddb1b-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ddb1b-143">Here is an example of the response.</span></span> 
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


