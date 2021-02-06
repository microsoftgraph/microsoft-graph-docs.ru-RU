---
title: Назначение типа ресурса tokenLifetimePolicy
description: Назначьте tokenLifetimePolicy приложению или основному приложению или службе.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1356714b5a54775ad304e6f32a063b2be7235954
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129074"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="35087-103">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="35087-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="35087-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35087-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35087-105">[Назначьте tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) [приложению](../resources/application.md) или [servicePrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="35087-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35087-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35087-106">Permissions</span></span>

<span data-ttu-id="35087-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35087-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35087-109">Permission type</span></span>                        | <span data-ttu-id="35087-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35087-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35087-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35087-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="35087-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35087-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="35087-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35087-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35087-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35087-114">Not supported.</span></span> |
| <span data-ttu-id="35087-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35087-115">Application</span></span>                            | <span data-ttu-id="35087-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35087-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35087-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35087-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="35087-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35087-118">Request headers</span></span>

| <span data-ttu-id="35087-119">Имя</span><span class="sxs-lookup"><span data-stu-id="35087-119">Name</span></span>          | <span data-ttu-id="35087-120">Описание</span><span class="sxs-lookup"><span data-stu-id="35087-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="35087-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35087-121">Authorization</span></span> | <span data-ttu-id="35087-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="35087-122">Bearer {token}</span></span> |
| <span data-ttu-id="35087-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35087-123">Content-Type</span></span> | <span data-ttu-id="35087-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35087-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="35087-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35087-125">Request body</span></span>

<span data-ttu-id="35087-126">В теле запроса укавите идентификатор объекта [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) (используя свойство), который должен быть назначен приложению или `@odata.id` основному приложению или службе.</span><span class="sxs-lookup"><span data-stu-id="35087-126">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="35087-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="35087-127">Response</span></span>

<span data-ttu-id="35087-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="35087-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35087-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="35087-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35087-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="35087-131">Request</span></span>

<span data-ttu-id="35087-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35087-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35087-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="35087-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="35087-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35087-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="35087-135">C#</span><span class="sxs-lookup"><span data-stu-id="35087-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35087-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35087-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35087-137">Java</span><span class="sxs-lookup"><span data-stu-id="35087-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35087-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="35087-138">Response</span></span>

<span data-ttu-id="35087-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35087-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



