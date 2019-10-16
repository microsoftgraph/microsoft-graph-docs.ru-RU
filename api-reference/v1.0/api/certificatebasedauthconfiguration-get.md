---
title: Получение Цертификатебаседаусконфигуратион
description: Получение свойств объекта цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e4a8a804b69a8840c4d2ed635d4d04cf55cbfe4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539234"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="df764-103">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="df764-103">Get certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="df764-104">Получение свойств объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="df764-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df764-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df764-105">Permissions</span></span>

<span data-ttu-id="df764-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df764-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df764-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df764-108">Permission type</span></span>                        | <span data-ttu-id="df764-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df764-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df764-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df764-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="df764-111">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df764-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="df764-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df764-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df764-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df764-113">Not supported.</span></span> |
| <span data-ttu-id="df764-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="df764-114">Application</span></span>    | <span data-ttu-id="df764-115">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df764-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df764-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df764-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="df764-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df764-117">Request headers</span></span>

| <span data-ttu-id="df764-118">Имя</span><span class="sxs-lookup"><span data-stu-id="df764-118">Name</span></span>      |<span data-ttu-id="df764-119">Описание</span><span class="sxs-lookup"><span data-stu-id="df764-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df764-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df764-120">Authorization</span></span> | <span data-ttu-id="df764-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df764-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df764-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df764-123">Request body</span></span>

<span data-ttu-id="df764-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df764-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df764-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="df764-125">Response</span></span>

<span data-ttu-id="df764-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df764-126">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df764-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="df764-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df764-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="df764-128">Request</span></span>

<span data-ttu-id="df764-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df764-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df764-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="df764-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```

---


### <a name="response"></a><span data-ttu-id="df764-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="df764-131">Response</span></span>

<span data-ttu-id="df764-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df764-132">The following is an example of the response.</span></span>

> <span data-ttu-id="df764-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df764-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
