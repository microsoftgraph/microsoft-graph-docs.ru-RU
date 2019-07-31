---
title: Удаление приложения
description: Удаляет приложение.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfc3fd437d81bcc9cdd8490f9597b409f87969a0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945580"
---
# <a name="delete-application"></a><span data-ttu-id="aa282-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="aa282-103">Delete application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa282-104">Удаляет приложение.</span><span class="sxs-lookup"><span data-stu-id="aa282-104">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa282-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa282-105">Permissions</span></span>
<span data-ttu-id="aa282-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa282-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa282-108">Permission type</span></span>      | <span data-ttu-id="aa282-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa282-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa282-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa282-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa282-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa282-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa282-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa282-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa282-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa282-113">Not supported.</span></span>    |
|<span data-ttu-id="aa282-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa282-114">Application</span></span> | <span data-ttu-id="aa282-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa282-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa282-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa282-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="aa282-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa282-117">Request headers</span></span>
| <span data-ttu-id="aa282-118">Имя</span><span class="sxs-lookup"><span data-stu-id="aa282-118">Name</span></span>       | <span data-ttu-id="aa282-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aa282-119">Type</span></span> | <span data-ttu-id="aa282-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aa282-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa282-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa282-121">Authorization</span></span>  | <span data-ttu-id="aa282-122">string</span><span class="sxs-lookup"><span data-stu-id="aa282-122">string</span></span>  | <span data-ttu-id="aa282-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa282-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa282-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa282-125">Request body</span></span>
<span data-ttu-id="aa282-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa282-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa282-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa282-127">Response</span></span>

<span data-ttu-id="aa282-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="aa282-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa282-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aa282-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa282-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa282-131">Request</span></span>
<span data-ttu-id="aa282-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa282-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aa282-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa282-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aa282-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa282-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa282-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa282-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aa282-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aa282-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aa282-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa282-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aa282-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa282-138">Response</span></span>
<span data-ttu-id="aa282-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa282-139">Here is an example of the response.</span></span> 
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
