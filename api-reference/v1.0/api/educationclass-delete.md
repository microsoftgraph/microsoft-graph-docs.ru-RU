---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9895666985b6179eeb5d5f266de515250d9339ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517617"
---
# <a name="delete-educationclass"></a><span data-ttu-id="2cb69-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="2cb69-104">Delete educationClass</span></span>

<span data-ttu-id="2cb69-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cb69-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cb69-106">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="2cb69-106">Delete a class.</span></span> <span data-ttu-id="2cb69-107">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="2cb69-107">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cb69-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cb69-108">Permissions</span></span>
<span data-ttu-id="2cb69-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cb69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cb69-111">Permission type</span></span>      | <span data-ttu-id="2cb69-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cb69-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cb69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cb69-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2cb69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cb69-114">Not supported.</span></span>  |
|<span data-ttu-id="2cb69-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cb69-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2cb69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cb69-116">Not supported.</span></span>  |
|<span data-ttu-id="2cb69-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cb69-117">Application</span></span> | <span data-ttu-id="2cb69-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb69-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2cb69-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cb69-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2cb69-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cb69-120">Request headers</span></span>
| <span data-ttu-id="2cb69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cb69-121">Header</span></span>       | <span data-ttu-id="2cb69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cb69-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2cb69-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cb69-123">Authorization</span></span>  | <span data-ttu-id="2cb69-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cb69-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2cb69-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cb69-126">Request body</span></span>
<span data-ttu-id="2cb69-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cb69-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2cb69-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cb69-128">Response</span></span>
<span data-ttu-id="2cb69-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2cb69-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cb69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2cb69-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cb69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cb69-132">Request</span></span>
<span data-ttu-id="2cb69-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cb69-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2cb69-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cb69-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="2cb69-135">C#</span><span class="sxs-lookup"><span data-stu-id="2cb69-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cb69-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cb69-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cb69-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cb69-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cb69-138">Java</span><span class="sxs-lookup"><span data-stu-id="2cb69-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2cb69-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cb69-139">Response</span></span>
<span data-ttu-id="2cb69-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2cb69-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
