---
title: Удаление приложения
description: Удаление объекта Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 942791a5c35d8a6202abab0cf7ab13ec7d9943df
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518926"
---
# <a name="delete-application"></a><span data-ttu-id="2e5ee-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="2e5ee-103">Delete application</span></span>

<span data-ttu-id="2e5ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e5ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e5ee-105">Удаление объекта [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="2e5ee-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e5ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5ee-106">Permissions</span></span>
<span data-ttu-id="2e5ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e5ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e5ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e5ee-109">Permission type</span></span>      | <span data-ttu-id="2e5ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e5ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e5ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e5ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e5ee-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e5ee-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e5ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e5ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-114">Not supported.</span></span>    |
|<span data-ttu-id="2e5ee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e5ee-115">Application</span></span> | <span data-ttu-id="2e5ee-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5ee-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e5ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e5ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e5ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e5ee-118">Request headers</span></span>
| <span data-ttu-id="2e5ee-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e5ee-119">Name</span></span>       | <span data-ttu-id="2e5ee-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2e5ee-120">Type</span></span> | <span data-ttu-id="2e5ee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2e5ee-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2e5ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5ee-122">Authorization</span></span>  | <span data-ttu-id="2e5ee-123">string</span><span class="sxs-lookup"><span data-stu-id="2e5ee-123">string</span></span>  | <span data-ttu-id="2e5ee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e5ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e5ee-126">Request body</span></span>
<span data-ttu-id="2e5ee-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e5ee-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5ee-128">Response</span></span>

<span data-ttu-id="2e5ee-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e5ee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e5ee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e5ee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e5ee-132">Request</span></span>
<span data-ttu-id="2e5ee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2e5ee-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e5ee-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="2e5ee-135">C#</span><span class="sxs-lookup"><span data-stu-id="2e5ee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e5ee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e5ee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e5ee-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e5ee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e5ee-138">Java</span><span class="sxs-lookup"><span data-stu-id="2e5ee-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e5ee-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e5ee-139">Response</span></span>
<span data-ttu-id="2e5ee-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e5ee-140">Here is an example of the response.</span></span> 
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
