---
title: Удаление registeredowners
description: Удаление пользователя в качестве зарегистрированного владельца устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eb4da89260b91ae96ecfd21bbf9f3266b0228084
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956463"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="3f5b1-103">Удаление registeredOwner</span><span class="sxs-lookup"><span data-stu-id="3f5b1-103">Delete registeredOwner</span></span>

<span data-ttu-id="3f5b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f5b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f5b1-105">Удаление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f5b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f5b1-106">Permissions</span></span>

<span data-ttu-id="3f5b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f5b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f5b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f5b1-109">Permission type</span></span>      | <span data-ttu-id="3f5b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f5b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f5b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f5b1-111">Delegated (work or school account)</span></span> |<span data-ttu-id="3f5b1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f5b1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f5b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f5b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f5b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-114">Not supported.</span></span>    |
|<span data-ttu-id="3f5b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f5b1-115">Application</span></span> | <span data-ttu-id="3f5b1-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f5b1-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="3f5b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f5b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3f5b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f5b1-118">Request headers</span></span>
| <span data-ttu-id="3f5b1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3f5b1-119">Name</span></span>       | <span data-ttu-id="3f5b1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3f5b1-120">Type</span></span> | <span data-ttu-id="3f5b1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3f5b1-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f5b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f5b1-122">Authorization</span></span>  | <span data-ttu-id="3f5b1-123">string</span><span class="sxs-lookup"><span data-stu-id="3f5b1-123">string</span></span>  | <span data-ttu-id="3f5b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f5b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f5b1-126">Request body</span></span>
<span data-ttu-id="3f5b1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f5b1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f5b1-128">Response</span></span>

<span data-ttu-id="3f5b1-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3f5b1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3f5b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f5b1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f5b1-131">Request</span></span>
<span data-ttu-id="3f5b1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f5b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f5b1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="3f5b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f5b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f5b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f5b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f5b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f5b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f5b1-137">Java</span><span class="sxs-lookup"><span data-stu-id="3f5b1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="3f5b1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f5b1-138">Response</span></span>
<span data-ttu-id="3f5b1-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f5b1-139">Here is an example of the response.</span></span>
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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


