---
title: Удаление servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bb1fc5a41baa29909c95b757208b12d8a1f8783b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334225"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="ae0e0-103">Удаление servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ae0e0-103">Delete servicePrincipal</span></span>

<span data-ttu-id="ae0e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae0e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae0e0-105">Удаление объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ae0e0-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae0e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0e0-106">Permissions</span></span>
<span data-ttu-id="ae0e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae0e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae0e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0e0-109">Permission type</span></span>      | <span data-ttu-id="ae0e0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae0e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae0e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae0e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae0e0-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ae0e0-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae0e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae0e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae0e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-114">Not supported.</span></span>    |
|<span data-ttu-id="ae0e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae0e0-115">Application</span></span> | <span data-ttu-id="ae0e0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae0e0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae0e0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae0e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ae0e0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae0e0-118">Request headers</span></span>
| <span data-ttu-id="ae0e0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae0e0-119">Name</span></span>       | <span data-ttu-id="ae0e0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae0e0-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ae0e0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae0e0-121">Authorization</span></span> | <span data-ttu-id="ae0e0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae0e0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae0e0-124">Content-type</span></span> | <span data-ttu-id="ae0e0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae0e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae0e0-127">Request body</span></span>
<span data-ttu-id="ae0e0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae0e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0e0-129">Response</span></span>

<span data-ttu-id="ae0e0-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae0e0-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae0e0-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="ae0e0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae0e0-133">Request</span></span>
<span data-ttu-id="ae0e0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae0e0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae0e0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="ae0e0-136">C#</span><span class="sxs-lookup"><span data-stu-id="ae0e0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae0e0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae0e0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae0e0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae0e0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae0e0-139">Java</span><span class="sxs-lookup"><span data-stu-id="ae0e0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ae0e0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0e0-140">Response</span></span>
<span data-ttu-id="ae0e0-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae0e0-141">Here is an example of the response.</span></span> 
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
