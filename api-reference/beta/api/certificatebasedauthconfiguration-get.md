---
title: Получение Цертификатебаседаусконфигуратион
description: Получение свойств объекта цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89da0fa3f569743dfe9bae31f2a30a00438794f2
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667669"
---
# <a name="get-certificatebasedauthconfiguration"></a><span data-ttu-id="4fbba-103">Получение Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4fbba-103">Get certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fbba-104">Получение свойств объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4fbba-104">Get the properties of a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fbba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fbba-105">Permissions</span></span>

<span data-ttu-id="4fbba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fbba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fbba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fbba-108">Permission type</span></span>                        | <span data-ttu-id="4fbba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fbba-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fbba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fbba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fbba-111">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4fbba-111">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="4fbba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fbba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fbba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fbba-113">Not supported.</span></span> |
| <span data-ttu-id="4fbba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fbba-114">Application</span></span>    | <span data-ttu-id="4fbba-115">Организация. чтение. ALL, Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4fbba-115">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fbba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fbba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4fbba-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fbba-117">Request headers</span></span>

| <span data-ttu-id="4fbba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4fbba-118">Name</span></span>      |<span data-ttu-id="4fbba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4fbba-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4fbba-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fbba-120">Authorization</span></span> | <span data-ttu-id="4fbba-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4fbba-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fbba-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fbba-122">Request body</span></span>

<span data-ttu-id="4fbba-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fbba-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fbba-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fbba-124">Response</span></span>

<span data-ttu-id="4fbba-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fbba-125">If successful, this method returns a `200 OK` response code and the requested [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fbba-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="4fbba-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fbba-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fbba-127">Request</span></span>

<span data-ttu-id="4fbba-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fbba-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfiguration"
}-->

```http
GET https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```

### <a name="response"></a><span data-ttu-id="4fbba-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fbba-129">Response</span></span>

<span data-ttu-id="4fbba-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4fbba-130">The following is an example of the response.</span></span>

> <span data-ttu-id="4fbba-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fbba-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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