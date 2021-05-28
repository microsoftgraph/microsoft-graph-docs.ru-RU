---
title: Удаление параметра группы
description: Удаление параметра группы.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f3b65b7f41e5a53ebada692347fdc53fbf986267
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679787"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="4830c-103">Удаление параметра группы</span><span class="sxs-lookup"><span data-stu-id="4830c-103">Delete a group setting</span></span>

<span data-ttu-id="4830c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4830c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4830c-105">Удаление параметра группы.</span><span class="sxs-lookup"><span data-stu-id="4830c-105">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="4830c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4830c-106">Permissions</span></span>

<span data-ttu-id="4830c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4830c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4830c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4830c-109">Permission type</span></span>      | <span data-ttu-id="4830c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4830c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4830c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4830c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4830c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4830c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4830c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4830c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4830c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4830c-114">Not supported.</span></span>    |
|<span data-ttu-id="4830c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4830c-115">Application</span></span> | <span data-ttu-id="4830c-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4830c-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4830c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4830c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="4830c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4830c-118">Request headers</span></span>

| <span data-ttu-id="4830c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4830c-119">Name</span></span> | <span data-ttu-id="4830c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4830c-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4830c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4830c-121">Authorization</span></span>  | <span data-ttu-id="4830c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4830c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4830c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4830c-124">Content-Type</span></span>  | <span data-ttu-id="4830c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4830c-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4830c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4830c-126">Request body</span></span>
<span data-ttu-id="4830c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4830c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4830c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4830c-128">Response</span></span>

<span data-ttu-id="4830c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4830c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4830c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4830c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4830c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4830c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4830c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4830c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="4830c-134">C#</span><span class="sxs-lookup"><span data-stu-id="4830c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4830c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4830c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4830c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4830c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4830c-137">Java</span><span class="sxs-lookup"><span data-stu-id="4830c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4830c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4830c-138">Response</span></span>
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

