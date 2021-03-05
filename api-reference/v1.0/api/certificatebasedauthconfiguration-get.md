---
title: Получить certificateBasedAuthConfiguration
description: Получите свойства объекта certificatebasedauthconfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 703de60a28c6339556c878b3e53b335bdb4f560c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434834"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="5c40e-103">Получить certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c40e-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="5c40e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c40e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c40e-105">Получите свойства объекта [certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c40e-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c40e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c40e-106">Permissions</span></span>

<span data-ttu-id="5c40e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c40e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c40e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c40e-109">Permission type</span></span>                        | <span data-ttu-id="5c40e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c40e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c40e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c40e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c40e-112">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c40e-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="5c40e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c40e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c40e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c40e-114">Not supported.</span></span> |
| <span data-ttu-id="5c40e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c40e-115">Application</span></span>    | <span data-ttu-id="5c40e-116">Organization.Read.All, Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c40e-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c40e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c40e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5c40e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c40e-118">Request headers</span></span>

| <span data-ttu-id="5c40e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c40e-119">Name</span></span>      |<span data-ttu-id="5c40e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c40e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c40e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c40e-121">Authorization</span></span> | <span data-ttu-id="5c40e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c40e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c40e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c40e-124">Request body</span></span>

<span data-ttu-id="5c40e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c40e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c40e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c40e-126">Response</span></span>

<span data-ttu-id="5c40e-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c40e-127">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c40e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c40e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c40e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c40e-129">Request</span></span>

<span data-ttu-id="5c40e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c40e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c40e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c40e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="5c40e-132">C#</span><span class="sxs-lookup"><span data-stu-id="5c40e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c40e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c40e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c40e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c40e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c40e-135">Java</span><span class="sxs-lookup"><span data-stu-id="5c40e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="5c40e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c40e-136">Response</span></span>

<span data-ttu-id="5c40e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c40e-137">The following is an example of the response.</span></span>

> <span data-ttu-id="5c40e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c40e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

