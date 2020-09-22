---
title: Удаление registeredUsers
description: Удаление пользователя в качестве зарегистрированного пользователя устройства.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36982981c5dcdf15526c5d163d7d088e8ce19326
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002564"
---
# <a name="delete-registereduser"></a><span data-ttu-id="91ca6-103">Удаление экземпляра registereduser</span><span class="sxs-lookup"><span data-stu-id="91ca6-103">Delete registeredUser</span></span>

<span data-ttu-id="91ca6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ca6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91ca6-105">Удаление пользователя в качестве зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="91ca6-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="91ca6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91ca6-106">Permissions</span></span>

<span data-ttu-id="91ca6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ca6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91ca6-109">Permission type</span></span>      | <span data-ttu-id="91ca6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91ca6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91ca6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91ca6-111">Delegated (work or school account)</span></span> |<span data-ttu-id="91ca6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91ca6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91ca6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91ca6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91ca6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91ca6-114">Not supported.</span></span>    |
|<span data-ttu-id="91ca6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91ca6-115">Application</span></span> | <span data-ttu-id="91ca6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ca6-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="91ca6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91ca6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="91ca6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91ca6-118">Request headers</span></span>
| <span data-ttu-id="91ca6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="91ca6-119">Name</span></span>       | <span data-ttu-id="91ca6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="91ca6-120">Type</span></span> | <span data-ttu-id="91ca6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="91ca6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="91ca6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91ca6-122">Authorization</span></span>  | <span data-ttu-id="91ca6-123">string</span><span class="sxs-lookup"><span data-stu-id="91ca6-123">string</span></span>  | <span data-ttu-id="91ca6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91ca6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91ca6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91ca6-126">Request body</span></span>
<span data-ttu-id="91ca6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91ca6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91ca6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="91ca6-128">Response</span></span>

<span data-ttu-id="91ca6-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91ca6-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91ca6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91ca6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91ca6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91ca6-131">Request</span></span>
<span data-ttu-id="91ca6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91ca6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91ca6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="91ca6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredUsers/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="91ca6-134">C#</span><span class="sxs-lookup"><span data-stu-id="91ca6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91ca6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91ca6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91ca6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91ca6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="91ca6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="91ca6-137">Response</span></span>
<span data-ttu-id="91ca6-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91ca6-138">Here is an example of the response.</span></span>
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


