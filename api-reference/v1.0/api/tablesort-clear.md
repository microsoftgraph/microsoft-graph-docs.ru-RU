---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 22a536cec56fee11f6bb20e47424a3eda389ba50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509473"
---
# <a name="tablesort-clear"></a><span data-ttu-id="234a4-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="234a4-104">TableSort: clear</span></span>

<span data-ttu-id="234a4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="234a4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="234a4-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="234a4-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="234a4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="234a4-108">Permissions</span></span>
<span data-ttu-id="234a4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="234a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="234a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="234a4-111">Permission type</span></span>      | <span data-ttu-id="234a4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="234a4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="234a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="234a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="234a4-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="234a4-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="234a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="234a4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="234a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234a4-116">Not supported.</span></span>    |
|<span data-ttu-id="234a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="234a4-117">Application</span></span> | <span data-ttu-id="234a4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234a4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="234a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="234a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="234a4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="234a4-120">Request headers</span></span>
| <span data-ttu-id="234a4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="234a4-121">Name</span></span>       | <span data-ttu-id="234a4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="234a4-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="234a4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="234a4-123">Authorization</span></span>  | <span data-ttu-id="234a4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="234a4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="234a4-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="234a4-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="234a4-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="234a4-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="234a4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="234a4-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="234a4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="234a4-130">Response</span></span>

<span data-ttu-id="234a4-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="234a4-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="234a4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="234a4-133">Example</span></span>
<span data-ttu-id="234a4-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="234a4-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="234a4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="234a4-135">Request</span></span>
<span data-ttu-id="234a4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="234a4-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="234a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="234a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="234a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="234a4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="234a4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="234a4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="234a4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="234a4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="234a4-141">Java</span><span class="sxs-lookup"><span data-stu-id="234a4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="234a4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="234a4-142">Response</span></span>
<span data-ttu-id="234a4-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="234a4-143">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
