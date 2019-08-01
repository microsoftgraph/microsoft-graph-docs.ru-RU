---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 39cc8f742da7a31edc45d3e0edb172b86e88ab11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024303"
---
# <a name="tablesort-clear"></a><span data-ttu-id="ab051-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="ab051-104">TableSort: clear</span></span>

<span data-ttu-id="ab051-p102">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="ab051-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab051-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab051-107">Permissions</span></span>
<span data-ttu-id="ab051-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab051-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab051-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab051-110">Permission type</span></span>      | <span data-ttu-id="ab051-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab051-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab051-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab051-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab051-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab051-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab051-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab051-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab051-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab051-115">Not supported.</span></span>    |
|<span data-ttu-id="ab051-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab051-116">Application</span></span> | <span data-ttu-id="ab051-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab051-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab051-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab051-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="ab051-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab051-119">Request headers</span></span>
| <span data-ttu-id="ab051-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ab051-120">Name</span></span>       | <span data-ttu-id="ab051-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ab051-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab051-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab051-122">Authorization</span></span>  | <span data-ttu-id="ab051-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab051-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab051-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ab051-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ab051-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ab051-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab051-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab051-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ab051-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab051-129">Response</span></span>

<span data-ttu-id="ab051-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ab051-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab051-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ab051-132">Example</span></span>
<span data-ttu-id="ab051-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ab051-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab051-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab051-134">Request</span></span>
<span data-ttu-id="ab051-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab051-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ab051-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab051-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab051-137">C#</span><span class="sxs-lookup"><span data-stu-id="ab051-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab051-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab051-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab051-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ab051-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ab051-140">Java</span><span class="sxs-lookup"><span data-stu-id="ab051-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab051-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab051-141">Response</span></span>
<span data-ttu-id="ab051-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab051-142">Here is an example of the response.</span></span> 
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
