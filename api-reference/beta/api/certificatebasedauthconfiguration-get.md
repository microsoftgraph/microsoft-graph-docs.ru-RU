---
title: Получение Цертификатебаседаусконфигуратион
description: Получение свойств объекта цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a315709cff9b8e3a64a5f4cde5f98d5c06093ea2
ms.sourcegitcommit: 25884c00cbfa2aa5c001cf777fd0ffa3c9a5ed68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36758309"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="a6889-103">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a6889-103">Get certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6889-104">Получение свойств объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a6889-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6889-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6889-105">Permissions</span></span>

<span data-ttu-id="a6889-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6889-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6889-108">Permission type</span></span>                        | <span data-ttu-id="a6889-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6889-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6889-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6889-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6889-111">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6889-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="a6889-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6889-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6889-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6889-113">Not supported.</span></span> |
| <span data-ttu-id="a6889-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6889-114">Application</span></span>    | <span data-ttu-id="a6889-115">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6889-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6889-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6889-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a6889-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6889-117">Request headers</span></span>

| <span data-ttu-id="a6889-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a6889-118">Name</span></span>      |<span data-ttu-id="a6889-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a6889-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6889-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6889-120">Authorization</span></span> | <span data-ttu-id="a6889-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a6889-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6889-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6889-122">Request body</span></span>

<span data-ttu-id="a6889-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6889-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6889-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6889-124">Response</span></span>

<span data-ttu-id="a6889-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6889-125">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6889-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6889-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6889-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6889-127">Request</span></span>

<span data-ttu-id="a6889-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6889-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6889-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6889-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6889-130">C#</span><span class="sxs-lookup"><span data-stu-id="a6889-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6889-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6889-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6889-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a6889-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6889-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6889-133">Response</span></span>

<span data-ttu-id="a6889-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6889-134">The following is an example of the response.</span></span>

> <span data-ttu-id="a6889-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6889-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
