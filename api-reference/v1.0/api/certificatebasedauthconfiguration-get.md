---
title: Получение Цертификатебаседаусконфигуратион
description: Получение свойств объекта цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d21f7e5824b1144234d2f3371eab53f2f835e4cc
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632571"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="96ed9-103">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="96ed9-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="96ed9-104">Получение свойств объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="96ed9-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96ed9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96ed9-105">Permissions</span></span>

<span data-ttu-id="96ed9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96ed9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96ed9-108">Permission type</span></span>                        | <span data-ttu-id="96ed9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96ed9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96ed9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96ed9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="96ed9-111">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="96ed9-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="96ed9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96ed9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96ed9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ed9-113">Not supported.</span></span> |
| <span data-ttu-id="96ed9-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="96ed9-114">Application</span></span>    | <span data-ttu-id="96ed9-115">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="96ed9-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96ed9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96ed9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96ed9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96ed9-117">Request headers</span></span>

| <span data-ttu-id="96ed9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="96ed9-118">Name</span></span>      |<span data-ttu-id="96ed9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="96ed9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96ed9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96ed9-120">Authorization</span></span> | <span data-ttu-id="96ed9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96ed9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96ed9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96ed9-123">Request body</span></span>

<span data-ttu-id="96ed9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96ed9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96ed9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="96ed9-125">Response</span></span>

<span data-ttu-id="96ed9-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96ed9-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96ed9-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="96ed9-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96ed9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="96ed9-128">Request</span></span>

<span data-ttu-id="96ed9-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96ed9-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96ed9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="96ed9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96ed9-131">C#</span><span class="sxs-lookup"><span data-stu-id="96ed9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96ed9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96ed9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96ed9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96ed9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96ed9-134">Java</span><span class="sxs-lookup"><span data-stu-id="96ed9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="96ed9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="96ed9-135">Response</span></span>

<span data-ttu-id="96ed9-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96ed9-136">The following is an example of the response.</span></span>

> <span data-ttu-id="96ed9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96ed9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
