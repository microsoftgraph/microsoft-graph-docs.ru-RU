---
title: Удаление параметра группы
description: Удаление параметра группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3c4d27271c3dc8f5af6170fe4ad7ed008438e1d5
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124611"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="35e69-103">Удаление параметра группы</span><span class="sxs-lookup"><span data-stu-id="35e69-103">Delete a group setting</span></span>

<span data-ttu-id="35e69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35e69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35e69-105">Удаление параметра группы.</span><span class="sxs-lookup"><span data-stu-id="35e69-105">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="35e69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35e69-106">Permissions</span></span>

<span data-ttu-id="35e69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="35e69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35e69-109">Permission type</span></span>      | <span data-ttu-id="35e69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35e69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35e69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35e69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35e69-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35e69-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35e69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35e69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35e69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e69-114">Not supported.</span></span>    |
|<span data-ttu-id="35e69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35e69-115">Application</span></span> | <span data-ttu-id="35e69-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35e69-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35e69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35e69-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="35e69-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35e69-118">Request headers</span></span>

| <span data-ttu-id="35e69-119">Имя</span><span class="sxs-lookup"><span data-stu-id="35e69-119">Name</span></span> | <span data-ttu-id="35e69-120">Описание</span><span class="sxs-lookup"><span data-stu-id="35e69-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="35e69-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35e69-121">Authorization</span></span>  | <span data-ttu-id="35e69-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35e69-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35e69-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35e69-124">Content-Type</span></span>  | <span data-ttu-id="35e69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35e69-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e69-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35e69-126">Request body</span></span>
<span data-ttu-id="35e69-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35e69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35e69-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="35e69-128">Response</span></span>

<span data-ttu-id="35e69-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="35e69-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35e69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="35e69-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35e69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="35e69-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="35e69-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="35e69-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="35e69-134">C#</span><span class="sxs-lookup"><span data-stu-id="35e69-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35e69-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35e69-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35e69-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35e69-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35e69-137">Java</span><span class="sxs-lookup"><span data-stu-id="35e69-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35e69-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="35e69-138">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
