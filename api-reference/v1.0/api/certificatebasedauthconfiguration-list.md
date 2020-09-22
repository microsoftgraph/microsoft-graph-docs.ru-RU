---
title: Список Цертификатебаседаусконфигуратионс
description: Получение списка объектов цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b230da9d17a934e40edc90767f30ba859a488e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992441"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="c018e-103">Список Цертификатебаседаусконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="c018e-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="c018e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c018e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c018e-105">Получение списка объектов [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c018e-105">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="c018e-106">В коллекции может существовать только один экземпляр Цертификатебаседаусконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="c018e-106">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="c018e-107">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="c018e-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="c018e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c018e-108">Permissions</span></span>

<span data-ttu-id="c018e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c018e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c018e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c018e-111">Permission type</span></span>                        | <span data-ttu-id="c018e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c018e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c018e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c018e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c018e-114">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c018e-114">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c018e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c018e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c018e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c018e-116">Not supported.</span></span> |
| <span data-ttu-id="c018e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c018e-117">Application</span></span>    | <span data-ttu-id="c018e-118">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c018e-118">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c018e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c018e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c018e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c018e-120">Request headers</span></span>

| <span data-ttu-id="c018e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c018e-121">Name</span></span>      |<span data-ttu-id="c018e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c018e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c018e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c018e-123">Authorization</span></span> | <span data-ttu-id="c018e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c018e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c018e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c018e-126">Request body</span></span>

<span data-ttu-id="c018e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c018e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c018e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c018e-128">Response</span></span>

<span data-ttu-id="c018e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c018e-129">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c018e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c018e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c018e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c018e-131">Request</span></span>

<span data-ttu-id="c018e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c018e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c018e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c018e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```
# <a name="c"></a>[<span data-ttu-id="c018e-134">C#</span><span class="sxs-lookup"><span data-stu-id="c018e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-certificatebasedauthconfigurations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c018e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c018e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-certificatebasedauthconfigurations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c018e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c018e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-certificatebasedauthconfigurations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c018e-137">Java</span><span class="sxs-lookup"><span data-stu-id="c018e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-certificatebasedauthconfigurations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="c018e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c018e-138">Response</span></span>

<span data-ttu-id="c018e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c018e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c018e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c018e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

