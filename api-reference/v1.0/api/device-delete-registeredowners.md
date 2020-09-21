---
title: Удаление registeredOwners
description: Удаление пользователя в качестве зарегистрированного владельца устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: afad1b2c93d552cbb3dfe2f63dc0509fd3faf5d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013407"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="0b048-103">Удаление registeredOwner</span><span class="sxs-lookup"><span data-stu-id="0b048-103">Delete registeredOwner</span></span>

<span data-ttu-id="0b048-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b048-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b048-105">Удаление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="0b048-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b048-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b048-106">Permissions</span></span>

<span data-ttu-id="0b048-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b048-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b048-109">Permission type</span></span>      | <span data-ttu-id="0b048-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b048-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b048-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b048-111">Delegated (work or school account)</span></span> |<span data-ttu-id="0b048-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b048-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b048-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b048-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b048-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b048-114">Not supported.</span></span>    |
|<span data-ttu-id="0b048-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b048-115">Application</span></span> | <span data-ttu-id="0b048-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b048-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0b048-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b048-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0b048-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b048-118">Request headers</span></span>
| <span data-ttu-id="0b048-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0b048-119">Name</span></span>       | <span data-ttu-id="0b048-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0b048-120">Type</span></span> | <span data-ttu-id="0b048-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0b048-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0b048-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b048-122">Authorization</span></span>  | <span data-ttu-id="0b048-123">string</span><span class="sxs-lookup"><span data-stu-id="0b048-123">string</span></span>  | <span data-ttu-id="0b048-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b048-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b048-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b048-126">Request body</span></span>
<span data-ttu-id="0b048-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b048-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b048-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b048-128">Response</span></span>

<span data-ttu-id="0b048-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b048-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b048-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0b048-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b048-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b048-131">Request</span></span>
<span data-ttu-id="0b048-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b048-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b048-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b048-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0b048-134">C#</span><span class="sxs-lookup"><span data-stu-id="0b048-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b048-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b048-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b048-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b048-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b048-137">Java</span><span class="sxs-lookup"><span data-stu-id="0b048-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="0b048-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b048-138">Response</span></span>
<span data-ttu-id="0b048-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b048-139">Here is an example of the response.</span></span>
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

