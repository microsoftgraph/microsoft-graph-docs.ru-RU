---
title: Удалить servicePrincipal
description: Удаление servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 7066cd3184894f8de1cada2f1936ee1bd343d4a0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137531"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="dbd67-103">Удалить servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="dbd67-103">Delete servicePrincipal</span></span>

<span data-ttu-id="dbd67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbd67-105">Удаление объекта [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="dbd67-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbd67-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbd67-106">Permissions</span></span>
<span data-ttu-id="dbd67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbd67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbd67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbd67-109">Permission type</span></span>      | <span data-ttu-id="dbd67-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbd67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbd67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbd67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbd67-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbd67-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="dbd67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbd67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbd67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbd67-114">Not supported.</span></span>    |
|<span data-ttu-id="dbd67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbd67-115">Application</span></span> | <span data-ttu-id="dbd67-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbd67-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbd67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbd67-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dbd67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbd67-118">Request headers</span></span>
| <span data-ttu-id="dbd67-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dbd67-119">Name</span></span>       | <span data-ttu-id="dbd67-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dbd67-120">Type</span></span> | <span data-ttu-id="dbd67-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dbd67-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbd67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbd67-122">Authorization</span></span>  | <span data-ttu-id="dbd67-123">string</span><span class="sxs-lookup"><span data-stu-id="dbd67-123">string</span></span>  | <span data-ttu-id="dbd67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbd67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbd67-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbd67-126">Request body</span></span>
<span data-ttu-id="dbd67-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbd67-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbd67-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd67-128">Response</span></span>

<span data-ttu-id="dbd67-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dbd67-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dbd67-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="dbd67-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="dbd67-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbd67-132">Request</span></span>
<span data-ttu-id="dbd67-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbd67-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dbd67-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbd67-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="dbd67-135">C#</span><span class="sxs-lookup"><span data-stu-id="dbd67-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbd67-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbd67-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbd67-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbd67-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dbd67-138">Java</span><span class="sxs-lookup"><span data-stu-id="dbd67-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dbd67-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbd67-139">Response</span></span>
<span data-ttu-id="dbd67-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dbd67-140">Here is an example of the response.</span></span> 
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



