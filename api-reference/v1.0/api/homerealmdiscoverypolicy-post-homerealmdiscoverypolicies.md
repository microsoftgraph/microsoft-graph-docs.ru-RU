---
title: Создание homeRealmDiscoveryPolicy
description: Создайте новый homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 31b201ea19658361cdb2bf7c3da2326c3e710e29
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051391"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="afc5e-103">Создание homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="afc5e-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="afc5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afc5e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="afc5e-105">Создайте новый [объект homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afc5e-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afc5e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afc5e-106">Permissions</span></span>

<span data-ttu-id="afc5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afc5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afc5e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afc5e-109">Permission type</span></span>                        | <span data-ttu-id="afc5e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afc5e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afc5e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afc5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="afc5e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="afc5e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="afc5e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afc5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afc5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afc5e-114">Not supported.</span></span> |
| <span data-ttu-id="afc5e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afc5e-115">Application</span></span>                            | <span data-ttu-id="afc5e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="afc5e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="afc5e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afc5e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="afc5e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afc5e-118">Request headers</span></span>

| <span data-ttu-id="afc5e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="afc5e-119">Name</span></span>          | <span data-ttu-id="afc5e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="afc5e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="afc5e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="afc5e-121">Authorization</span></span> | <span data-ttu-id="afc5e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afc5e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="afc5e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afc5e-124">Content-type</span></span> | <span data-ttu-id="afc5e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afc5e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afc5e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afc5e-127">Request body</span></span>

<span data-ttu-id="afc5e-128">В теле запроса поставляем JSON представление [объекта homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afc5e-128">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="afc5e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="afc5e-129">Response</span></span>

<span data-ttu-id="afc5e-130">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="afc5e-130">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afc5e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="afc5e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afc5e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afc5e-132">Request</span></span>

<span data-ttu-id="afc5e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afc5e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="afc5e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="afc5e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="afc5e-135">C#</span><span class="sxs-lookup"><span data-stu-id="afc5e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afc5e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afc5e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afc5e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afc5e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afc5e-138">Java</span><span class="sxs-lookup"><span data-stu-id="afc5e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afc5e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="afc5e-139">Response</span></span>

<span data-ttu-id="afc5e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="afc5e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="afc5e-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="afc5e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

