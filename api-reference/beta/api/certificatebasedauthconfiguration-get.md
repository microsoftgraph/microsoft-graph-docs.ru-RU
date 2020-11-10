---
title: Получение Цертификатебаседаусконфигуратион
description: Получение свойств объекта цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a00e2638050c5a648e98e9e2edf297fa6662cc46
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959417"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="029af-103">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="029af-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="029af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="029af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="029af-105">Получение свойств объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="029af-105">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="029af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="029af-106">Permissions</span></span>

<span data-ttu-id="029af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="029af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="029af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="029af-109">Permission type</span></span>                        | <span data-ttu-id="029af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="029af-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="029af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="029af-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="029af-112">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="029af-112">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="029af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="029af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="029af-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="029af-114">Not supported.</span></span> |
| <span data-ttu-id="029af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="029af-115">Application</span></span>    | <span data-ttu-id="029af-116">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="029af-116">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="029af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="029af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="029af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="029af-118">Request headers</span></span>

| <span data-ttu-id="029af-119">Имя</span><span class="sxs-lookup"><span data-stu-id="029af-119">Name</span></span>      |<span data-ttu-id="029af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="029af-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="029af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="029af-121">Authorization</span></span> | <span data-ttu-id="029af-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="029af-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="029af-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="029af-123">Request body</span></span>

<span data-ttu-id="029af-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="029af-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="029af-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="029af-125">Response</span></span>

<span data-ttu-id="029af-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="029af-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="029af-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="029af-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="029af-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="029af-128">Request</span></span>

<span data-ttu-id="029af-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="029af-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="029af-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="029af-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="029af-131">C#</span><span class="sxs-lookup"><span data-stu-id="029af-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="029af-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="029af-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="029af-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="029af-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="029af-134">Java</span><span class="sxs-lookup"><span data-stu-id="029af-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="029af-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="029af-135">Response</span></span>

<span data-ttu-id="029af-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="029af-136">The following is an example of the response.</span></span>

> <span data-ttu-id="029af-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="029af-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


