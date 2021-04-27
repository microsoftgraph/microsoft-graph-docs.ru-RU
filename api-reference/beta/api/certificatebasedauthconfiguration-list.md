---
title: List certificateBasedAuthConfigurations
description: Получите список объектов certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b2a858bcd1d504f774da17e65bfa4657216e8730
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047562"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="d83de-103">List certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="d83de-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="d83de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d83de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d83de-105">Получите список [объектов certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d83de-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="d83de-106">В коллекции может существовать только один экземпляр certificateBasedAuthConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d83de-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="d83de-107">Он всегда имеет фиксированный ID со значением '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="d83de-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="d83de-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d83de-108">Permissions</span></span>

<span data-ttu-id="d83de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d83de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d83de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d83de-111">Permission type</span></span>                        | <span data-ttu-id="d83de-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d83de-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d83de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d83de-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d83de-114">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83de-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="d83de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d83de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d83de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d83de-116">Not supported.</span></span> |
| <span data-ttu-id="d83de-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d83de-117">Application</span></span>    | <span data-ttu-id="d83de-118">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d83de-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d83de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d83de-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="d83de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d83de-120">Request headers</span></span>

| <span data-ttu-id="d83de-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d83de-121">Name</span></span>      |<span data-ttu-id="d83de-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d83de-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d83de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d83de-123">Authorization</span></span> | <span data-ttu-id="d83de-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d83de-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d83de-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d83de-125">Request body</span></span>

<span data-ttu-id="d83de-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d83de-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d83de-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d83de-127">Response</span></span>

<span data-ttu-id="d83de-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d83de-128">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d83de-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="d83de-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d83de-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d83de-130">Request</span></span>

<span data-ttu-id="d83de-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d83de-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d83de-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d83de-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="d83de-133">C#</span><span class="sxs-lookup"><span data-stu-id="d83de-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d83de-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d83de-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d83de-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d83de-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d83de-136">Java</span><span class="sxs-lookup"><span data-stu-id="d83de-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d83de-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d83de-137">Response</span></span>

<span data-ttu-id="d83de-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d83de-138">The following is an example of the response.</span></span>

> <span data-ttu-id="d83de-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d83de-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "certificateAuthorities": [
        {
          "isRootAuthority": true,
          "certificateRevocationListUrl": "CRLUrl-value",
          "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
          "certificate": "Binary",
          "issuer": "issuer-value",
          "issuerSki": "issuerSki-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


