---
title: Список Цертификатебаседаусконфигуратионс
description: Получение списка объектов цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f045eee24c9c4150419e69adc7279987206510d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518632"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="5a6bf-103">Список Цертификатебаседаусконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="5a6bf-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="5a6bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a6bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a6bf-105">Получение списка объектов [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5a6bf-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="5a6bf-106">В коллекции может существовать только один экземпляр Цертификатебаседаусконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="5a6bf-107">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="5a6bf-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a6bf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6bf-108">Permissions</span></span>

<span data-ttu-id="5a6bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a6bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a6bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a6bf-111">Permission type</span></span>                        | <span data-ttu-id="5a6bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a6bf-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5a6bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a6bf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a6bf-114">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a6bf-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="5a6bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a6bf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a6bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-116">Not supported.</span></span> |
| <span data-ttu-id="5a6bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a6bf-117">Application</span></span>    | <span data-ttu-id="5a6bf-118">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a6bf-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a6bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a6bf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="5a6bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a6bf-120">Request headers</span></span>

| <span data-ttu-id="5a6bf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5a6bf-121">Name</span></span>      |<span data-ttu-id="5a6bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a6bf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a6bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a6bf-123">Authorization</span></span> | <span data-ttu-id="5a6bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a6bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a6bf-126">Request body</span></span>

<span data-ttu-id="5a6bf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a6bf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a6bf-128">Response</span></span>

<span data-ttu-id="5a6bf-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-129">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a6bf-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a6bf-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a6bf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a6bf-131">Request</span></span>

<span data-ttu-id="5a6bf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a6bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a6bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="5a6bf-134">C#</span><span class="sxs-lookup"><span data-stu-id="5a6bf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a6bf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a6bf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a6bf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a6bf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a6bf-137">Java</span><span class="sxs-lookup"><span data-stu-id="5a6bf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="5a6bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a6bf-138">Response</span></span>

<span data-ttu-id="5a6bf-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-139">The following is an example of the response.</span></span>

> <span data-ttu-id="5a6bf-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a6bf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
