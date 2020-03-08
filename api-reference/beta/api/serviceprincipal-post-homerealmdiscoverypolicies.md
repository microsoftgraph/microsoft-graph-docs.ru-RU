---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте Хомереалмдисковериполици участнику службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6633fdf13818a2b9af5b8968a1e82e5a4315b83f
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562810"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="36dc5-103">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="36dc5-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="36dc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36dc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36dc5-105">Назначьте [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="36dc5-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36dc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36dc5-106">Permissions</span></span>

<span data-ttu-id="36dc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36dc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36dc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36dc5-109">Permission type</span></span>                        | <span data-ttu-id="36dc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36dc5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36dc5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36dc5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36dc5-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="36dc5-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="36dc5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36dc5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36dc5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36dc5-114">Not supported.</span></span> |
| <span data-ttu-id="36dc5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36dc5-115">Application</span></span>                            | <span data-ttu-id="36dc5-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="36dc5-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36dc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36dc5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="36dc5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36dc5-118">Request headers</span></span>

| <span data-ttu-id="36dc5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="36dc5-119">Name</span></span>          | <span data-ttu-id="36dc5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="36dc5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36dc5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36dc5-121">Authorization</span></span> | <span data-ttu-id="36dc5-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="36dc5-122">Bearer {token}</span></span> |
| <span data-ttu-id="36dc5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36dc5-123">Content-Type</span></span> | <span data-ttu-id="36dc5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36dc5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="36dc5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36dc5-125">Request body</span></span>

<span data-ttu-id="36dc5-126">В тексте запроса укажите идентификатор объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="36dc5-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="36dc5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="36dc5-127">Response</span></span>

<span data-ttu-id="36dc5-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="36dc5-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36dc5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="36dc5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36dc5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36dc5-131">Request</span></span>

<span data-ttu-id="36dc5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36dc5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36dc5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36dc5-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="36dc5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36dc5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36dc5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="36dc5-135">Response</span></span>

<span data-ttu-id="36dc5-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36dc5-136">The following is an example of the response.</span></span>

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
