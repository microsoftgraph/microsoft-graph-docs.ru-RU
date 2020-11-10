---
title: Удалить servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 96464d54e6dee547b6c67903d5f833c874868919
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969646"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="ff65d-103">Удалить servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="ff65d-103">Delete servicePrincipal</span></span>

<span data-ttu-id="ff65d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff65d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff65d-105">Удаление объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ff65d-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff65d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff65d-106">Permissions</span></span>
<span data-ttu-id="ff65d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff65d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff65d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff65d-109">Permission type</span></span>      | <span data-ttu-id="ff65d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff65d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff65d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff65d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff65d-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff65d-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="ff65d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff65d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff65d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff65d-114">Not supported.</span></span>    |
|<span data-ttu-id="ff65d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff65d-115">Application</span></span> | <span data-ttu-id="ff65d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff65d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff65d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff65d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ff65d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff65d-118">Request headers</span></span>
| <span data-ttu-id="ff65d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ff65d-119">Name</span></span>       | <span data-ttu-id="ff65d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ff65d-120">Type</span></span> | <span data-ttu-id="ff65d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff65d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff65d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff65d-122">Authorization</span></span>  | <span data-ttu-id="ff65d-123">string</span><span class="sxs-lookup"><span data-stu-id="ff65d-123">string</span></span>  | <span data-ttu-id="ff65d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff65d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff65d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff65d-126">Request body</span></span>
<span data-ttu-id="ff65d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff65d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff65d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff65d-128">Response</span></span>

<span data-ttu-id="ff65d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ff65d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff65d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff65d-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="ff65d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff65d-132">Request</span></span>
<span data-ttu-id="ff65d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff65d-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff65d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff65d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="ff65d-135">C#</span><span class="sxs-lookup"><span data-stu-id="ff65d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff65d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff65d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff65d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff65d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff65d-138">Java</span><span class="sxs-lookup"><span data-stu-id="ff65d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ff65d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff65d-139">Response</span></span>
<span data-ttu-id="ff65d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ff65d-140">Here is an example of the response.</span></span> 
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


