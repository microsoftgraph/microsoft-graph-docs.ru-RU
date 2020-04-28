---
title: Удаление приложения
description: Удаляет приложение.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e420eb81346b56e969a745124e09fe6607c3e13b
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107208"
---
# <a name="delete-application"></a><span data-ttu-id="860df-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="860df-103">Delete application</span></span>

<span data-ttu-id="860df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="860df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="860df-105">Удаляет приложение.</span><span class="sxs-lookup"><span data-stu-id="860df-105">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="860df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="860df-106">Permissions</span></span>
<span data-ttu-id="860df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="860df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="860df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="860df-109">Permission type</span></span>      | <span data-ttu-id="860df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="860df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="860df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="860df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="860df-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="860df-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="860df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="860df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="860df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="860df-114">Not supported.</span></span>    |
|<span data-ttu-id="860df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="860df-115">Application</span></span> | <span data-ttu-id="860df-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="860df-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="860df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="860df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="860df-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="860df-118">Request headers</span></span>
| <span data-ttu-id="860df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="860df-119">Name</span></span>       | <span data-ttu-id="860df-120">Тип</span><span class="sxs-lookup"><span data-stu-id="860df-120">Type</span></span> | <span data-ttu-id="860df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="860df-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="860df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="860df-122">Authorization</span></span>  | <span data-ttu-id="860df-123">string</span><span class="sxs-lookup"><span data-stu-id="860df-123">string</span></span>  | <span data-ttu-id="860df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="860df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="860df-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="860df-126">Request body</span></span>
<span data-ttu-id="860df-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="860df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="860df-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="860df-128">Response</span></span>

<span data-ttu-id="860df-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="860df-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="860df-131">Пример</span><span class="sxs-lookup"><span data-stu-id="860df-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="860df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="860df-132">Request</span></span>
<span data-ttu-id="860df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="860df-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="860df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="860df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="860df-135">C#</span><span class="sxs-lookup"><span data-stu-id="860df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="860df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="860df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="860df-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="860df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="860df-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="860df-138">Response</span></span>
<span data-ttu-id="860df-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="860df-139">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
