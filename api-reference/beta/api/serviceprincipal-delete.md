---
title: Удаление servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: cad7df48a955dbe06a239b120d6b32f079a7043b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219307"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="aa57a-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="aa57a-103">Delete servicePrincipal</span></span>

<span data-ttu-id="aa57a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa57a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa57a-105">Удаление servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="aa57a-105">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa57a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa57a-106">Permissions</span></span>
<span data-ttu-id="aa57a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa57a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa57a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa57a-109">Permission type</span></span>      | <span data-ttu-id="aa57a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa57a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa57a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa57a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa57a-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa57a-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa57a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa57a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa57a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa57a-114">Not supported.</span></span>    |
|<span data-ttu-id="aa57a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa57a-115">Application</span></span> | <span data-ttu-id="aa57a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa57a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa57a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa57a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="aa57a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa57a-118">Request headers</span></span>
| <span data-ttu-id="aa57a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aa57a-119">Name</span></span>       | <span data-ttu-id="aa57a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="aa57a-120">Type</span></span> | <span data-ttu-id="aa57a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="aa57a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa57a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa57a-122">Authorization</span></span>  | <span data-ttu-id="aa57a-123">string</span><span class="sxs-lookup"><span data-stu-id="aa57a-123">string</span></span>  | <span data-ttu-id="aa57a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa57a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa57a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa57a-126">Request body</span></span>
<span data-ttu-id="aa57a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa57a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa57a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa57a-128">Response</span></span>

<span data-ttu-id="aa57a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="aa57a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa57a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa57a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa57a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa57a-132">Request</span></span>
<span data-ttu-id="aa57a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa57a-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa57a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa57a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="aa57a-135">C#</span><span class="sxs-lookup"><span data-stu-id="aa57a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa57a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa57a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa57a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa57a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aa57a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa57a-138">Response</span></span>
<span data-ttu-id="aa57a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa57a-139">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
