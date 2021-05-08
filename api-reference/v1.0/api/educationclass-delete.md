---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4f3d509364168227766465ead899340b00f24f83
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232027"
---
# <a name="delete-educationclass"></a><span data-ttu-id="86201-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="86201-104">Delete educationClass</span></span>

<span data-ttu-id="86201-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86201-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86201-106">Удаление [образовательного класса](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="86201-106">Delete an [educationClass](../resources/educationclass.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="86201-107">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="86201-107">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="86201-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86201-108">Permissions</span></span>
<span data-ttu-id="86201-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86201-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86201-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86201-111">Permission type</span></span>      | <span data-ttu-id="86201-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86201-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86201-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86201-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="86201-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86201-114">Not supported.</span></span>  |
|<span data-ttu-id="86201-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86201-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="86201-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86201-116">Not supported.</span></span>  |
|<span data-ttu-id="86201-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="86201-117">Application</span></span> | <span data-ttu-id="86201-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86201-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86201-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86201-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="86201-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86201-120">Request headers</span></span>
| <span data-ttu-id="86201-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86201-121">Header</span></span>       | <span data-ttu-id="86201-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86201-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86201-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86201-123">Authorization</span></span>  | <span data-ttu-id="86201-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86201-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86201-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86201-126">Request body</span></span>
<span data-ttu-id="86201-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86201-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="86201-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="86201-128">Response</span></span>
<span data-ttu-id="86201-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86201-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86201-131">Пример</span><span class="sxs-lookup"><span data-stu-id="86201-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86201-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86201-132">Request</span></span>
<span data-ttu-id="86201-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86201-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86201-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="86201-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="86201-135">C#</span><span class="sxs-lookup"><span data-stu-id="86201-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86201-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86201-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86201-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86201-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86201-138">Java</span><span class="sxs-lookup"><span data-stu-id="86201-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86201-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="86201-139">Response</span></span>
<span data-ttu-id="86201-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="86201-140">The following is an example of the response.</span></span> 

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
