---
title: Список Цертификатебаседаусконфигуратионс
description: Получение списка объектов цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13380b1d1156a2a388ea5b12f48f27077006af12
ms.sourcegitcommit: 25884c00cbfa2aa5c001cf777fd0ffa3c9a5ed68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36758295"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="de240-103">Список Цертификатебаседаусконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="de240-103">List certificateBasedAuthConfigurations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de240-104">Получение списка объектов [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="de240-104">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="de240-105">В коллекции может существовать только один экземпляр Цертификатебаседаусконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="de240-105">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="de240-106">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="de240-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="de240-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de240-107">Permissions</span></span>

<span data-ttu-id="de240-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de240-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de240-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de240-110">Permission type</span></span>                        | <span data-ttu-id="de240-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de240-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de240-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de240-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de240-113">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de240-113">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="de240-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de240-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de240-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de240-115">Not supported.</span></span> |
| <span data-ttu-id="de240-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de240-116">Application</span></span>    | <span data-ttu-id="de240-117">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="de240-117">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de240-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de240-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="de240-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de240-119">Request headers</span></span>

| <span data-ttu-id="de240-120">Имя</span><span class="sxs-lookup"><span data-stu-id="de240-120">Name</span></span>      |<span data-ttu-id="de240-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de240-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de240-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de240-122">Authorization</span></span> | <span data-ttu-id="de240-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="de240-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="de240-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de240-124">Request body</span></span>

<span data-ttu-id="de240-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de240-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de240-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="de240-126">Response</span></span>

<span data-ttu-id="de240-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de240-127">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de240-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="de240-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de240-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="de240-129">Request</span></span>

<span data-ttu-id="de240-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de240-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de240-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="de240-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de240-132">C#</span><span class="sxs-lookup"><span data-stu-id="de240-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de240-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de240-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de240-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="de240-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de240-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="de240-135">Response</span></span>

<span data-ttu-id="de240-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de240-136">The following is an example of the response.</span></span>

> <span data-ttu-id="de240-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de240-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
