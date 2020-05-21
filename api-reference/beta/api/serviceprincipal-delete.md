---
title: Удаление servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: f42a7bf4f4b9ddf4e0bb4161f602c48a76ced739
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335623"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="56206-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="56206-103">Delete servicePrincipal</span></span>

<span data-ttu-id="56206-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56206-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56206-105">Удаление объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="56206-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="56206-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56206-106">Permissions</span></span>
<span data-ttu-id="56206-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56206-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56206-109">Permission type</span></span>      | <span data-ttu-id="56206-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56206-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56206-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56206-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56206-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="56206-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="56206-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56206-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56206-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56206-114">Not supported.</span></span>    |
|<span data-ttu-id="56206-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56206-115">Application</span></span> | <span data-ttu-id="56206-116">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="56206-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56206-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56206-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="56206-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56206-118">Request headers</span></span>
| <span data-ttu-id="56206-119">Имя</span><span class="sxs-lookup"><span data-stu-id="56206-119">Name</span></span>       | <span data-ttu-id="56206-120">Тип</span><span class="sxs-lookup"><span data-stu-id="56206-120">Type</span></span> | <span data-ttu-id="56206-121">Описание</span><span class="sxs-lookup"><span data-stu-id="56206-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56206-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="56206-122">Authorization</span></span>  | <span data-ttu-id="56206-123">string</span><span class="sxs-lookup"><span data-stu-id="56206-123">string</span></span>  | <span data-ttu-id="56206-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56206-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56206-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56206-126">Request body</span></span>
<span data-ttu-id="56206-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56206-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56206-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="56206-128">Response</span></span>

<span data-ttu-id="56206-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="56206-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56206-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="56206-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="56206-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="56206-132">Request</span></span>
<span data-ttu-id="56206-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56206-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56206-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="56206-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="56206-135">C#</span><span class="sxs-lookup"><span data-stu-id="56206-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56206-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56206-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56206-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56206-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="56206-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="56206-138">Response</span></span>
<span data-ttu-id="56206-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56206-139">Here is an example of the response.</span></span> 
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
