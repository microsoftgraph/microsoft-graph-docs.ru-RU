---
title: Получить certificateBasedAuthConfiguration
description: Получите свойства объекта certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5009db18fd17ae160375f76db296f1d3f5a9c694
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047576"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="e32b4-103">Получить certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="e32b4-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="e32b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e32b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e32b4-105">Получите свойства объекта [certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e32b4-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e32b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e32b4-106">Permissions</span></span>

<span data-ttu-id="e32b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e32b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e32b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e32b4-109">Permission type</span></span>                        | <span data-ttu-id="e32b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e32b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e32b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e32b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e32b4-112">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32b4-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="e32b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e32b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e32b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e32b4-114">Not supported.</span></span> |
| <span data-ttu-id="e32b4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e32b4-115">Application</span></span>    | <span data-ttu-id="e32b4-116">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e32b4-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e32b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e32b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e32b4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e32b4-118">Request headers</span></span>

| <span data-ttu-id="e32b4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e32b4-119">Name</span></span>      |<span data-ttu-id="e32b4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e32b4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e32b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e32b4-121">Authorization</span></span> | <span data-ttu-id="e32b4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e32b4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e32b4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e32b4-123">Request body</span></span>

<span data-ttu-id="e32b4-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e32b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e32b4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32b4-125">Response</span></span>

<span data-ttu-id="e32b4-126">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e32b4-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e32b4-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="e32b4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e32b4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e32b4-128">Request</span></span>

<span data-ttu-id="e32b4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e32b4-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e32b4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e32b4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="e32b4-131">C#</span><span class="sxs-lookup"><span data-stu-id="e32b4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e32b4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e32b4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e32b4-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e32b4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e32b4-134">Java</span><span class="sxs-lookup"><span data-stu-id="e32b4-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e32b4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e32b4-135">Response</span></span>

<span data-ttu-id="e32b4-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e32b4-136">The following is an example of the response.</span></span>

> <span data-ttu-id="e32b4-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e32b4-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


