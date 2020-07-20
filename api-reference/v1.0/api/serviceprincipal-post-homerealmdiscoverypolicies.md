---
title: Назначение типа ресурса homeRealmDiscoveryPolicy
description: Назначьте Хомереалмдисковериполици для servicePrincipal.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f30ff49bfe43e67ee4ae7fbac21277c060244d02
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863945"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="a12af-103">Назначение типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="a12af-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="a12af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a12af-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a12af-105">Назначьте [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) для [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="a12af-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a12af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a12af-106">Permissions</span></span>

<span data-ttu-id="a12af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a12af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a12af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a12af-109">Permission type</span></span>                        | <span data-ttu-id="a12af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a12af-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a12af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a12af-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a12af-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a12af-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="a12af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a12af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a12af-114">Not supported.</span></span> |
| <span data-ttu-id="a12af-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a12af-115">Application</span></span>                            | <span data-ttu-id="a12af-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a12af-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a12af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a12af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a12af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a12af-118">Request headers</span></span>

| <span data-ttu-id="a12af-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a12af-119">Name</span></span>          | <span data-ttu-id="a12af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a12af-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a12af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a12af-121">Authorization</span></span> | <span data-ttu-id="a12af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a12af-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a12af-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a12af-124">Content-Type</span></span> | <span data-ttu-id="a12af-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a12af-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a12af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a12af-127">Request body</span></span>

<span data-ttu-id="a12af-128">В тексте запроса укажите идентификатор объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен субъекту-службе.</span><span class="sxs-lookup"><span data-stu-id="a12af-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="a12af-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a12af-129">Response</span></span>

<span data-ttu-id="a12af-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a12af-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a12af-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a12af-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a12af-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a12af-133">Request</span></span>

<span data-ttu-id="a12af-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a12af-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a12af-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a12af-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="a12af-136">C#</span><span class="sxs-lookup"><span data-stu-id="a12af-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a12af-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a12af-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a12af-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a12af-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a12af-139">Java</span><span class="sxs-lookup"><span data-stu-id="a12af-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a12af-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a12af-140">Response</span></span>

<span data-ttu-id="a12af-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a12af-141">The following is an example of the response.</span></span>

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
