---
title: Удаление registeredUsers
description: Удалите пользователя как зарегистрированного пользователя устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: edc51e2610a3692dfa70dee2f0d16b701df5f8bc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437233"
---
# <a name="delete-registereduser"></a><span data-ttu-id="0c1c9-103">Удаление registeredUser</span><span class="sxs-lookup"><span data-stu-id="0c1c9-103">Delete registeredUser</span></span>

<span data-ttu-id="0c1c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c1c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c1c9-105">Удалите пользователя как зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c1c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c1c9-106">Permissions</span></span>

<span data-ttu-id="0c1c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c1c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c1c9-109">Permission type</span></span>      | <span data-ttu-id="0c1c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c1c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c1c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c1c9-111">Delegated (work or school account)</span></span> |<span data-ttu-id="0c1c9-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c1c9-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c1c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c1c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c1c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-114">Not supported.</span></span>    |
|<span data-ttu-id="0c1c9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c1c9-115">Application</span></span> | <span data-ttu-id="0c1c9-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c1c9-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0c1c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c1c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0c1c9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c1c9-118">Request headers</span></span>
| <span data-ttu-id="0c1c9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c1c9-119">Name</span></span>       | <span data-ttu-id="0c1c9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0c1c9-120">Type</span></span> | <span data-ttu-id="0c1c9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0c1c9-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c1c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c1c9-122">Authorization</span></span>  | <span data-ttu-id="0c1c9-123">string</span><span class="sxs-lookup"><span data-stu-id="0c1c9-123">string</span></span>  | <span data-ttu-id="0c1c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c1c9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c1c9-126">Request body</span></span>
<span data-ttu-id="0c1c9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c1c9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c1c9-128">Response</span></span>

<span data-ttu-id="0c1c9-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c1c9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0c1c9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c1c9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c1c9-131">Request</span></span>
<span data-ttu-id="0c1c9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c1c9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c1c9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0c1c9-134">C#</span><span class="sxs-lookup"><span data-stu-id="0c1c9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c1c9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c1c9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c1c9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c1c9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c1c9-137">Java</span><span class="sxs-lookup"><span data-stu-id="0c1c9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredusers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="0c1c9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c1c9-138">Response</span></span>
<span data-ttu-id="0c1c9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c1c9-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


