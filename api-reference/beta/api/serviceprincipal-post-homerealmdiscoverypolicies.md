---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте homeRealmDiscoveryPolicy для основного службы.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 244b86ec441a64e5e58ef593eae332c10c2b3c6d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134185"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="daf14-103">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="daf14-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="daf14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daf14-105">[Назначьте homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) [servicePrincipal.](../resources/servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="daf14-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="daf14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daf14-106">Permissions</span></span>

<span data-ttu-id="daf14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daf14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="daf14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daf14-109">Permission type</span></span>                        | <span data-ttu-id="daf14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daf14-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="daf14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daf14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="daf14-112">Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf14-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="daf14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daf14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daf14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf14-114">Not supported.</span></span> |
| <span data-ttu-id="daf14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daf14-115">Application</span></span>                            | <span data-ttu-id="daf14-116">Policy.Read.All и Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.OwnedBy, Policy.Read.All и Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration и Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf14-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="daf14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daf14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="daf14-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daf14-118">Request headers</span></span>

| <span data-ttu-id="daf14-119">Имя</span><span class="sxs-lookup"><span data-stu-id="daf14-119">Name</span></span>          | <span data-ttu-id="daf14-120">Описание</span><span class="sxs-lookup"><span data-stu-id="daf14-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="daf14-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="daf14-121">Authorization</span></span> | <span data-ttu-id="daf14-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="daf14-122">Bearer {token}</span></span> |
| <span data-ttu-id="daf14-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daf14-123">Content-Type</span></span> | <span data-ttu-id="daf14-124">application/json</span><span class="sxs-lookup"><span data-stu-id="daf14-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="daf14-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daf14-125">Request body</span></span>

<span data-ttu-id="daf14-126">В теле запроса укавите идентификатор объекта [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) (используя свойство), который должен быть назначен основному `@odata.id` объекту-службе.</span><span class="sxs-lookup"><span data-stu-id="daf14-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="daf14-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="daf14-127">Response</span></span>

<span data-ttu-id="daf14-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="daf14-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daf14-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="daf14-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daf14-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="daf14-131">Request</span></span>

<span data-ttu-id="daf14-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daf14-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="daf14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="daf14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="daf14-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daf14-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="daf14-135">C#</span><span class="sxs-lookup"><span data-stu-id="daf14-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daf14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daf14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="daf14-137">Java</span><span class="sxs-lookup"><span data-stu-id="daf14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="daf14-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="daf14-138">Response</span></span>

<span data-ttu-id="daf14-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="daf14-139">The following is an example of the response.</span></span>

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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



