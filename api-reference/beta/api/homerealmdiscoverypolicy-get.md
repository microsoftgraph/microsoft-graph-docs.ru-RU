---
title: Получение Хомереалмдисковериполици
description: Получение свойств и связей объекта Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 665c489e45555ec4de2283ba50dd89af1def22f1
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234486"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="20a48-103">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="20a48-103">Get homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20a48-104">Получение свойств и связей объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="20a48-104">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20a48-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20a48-105">Permissions</span></span>

<span data-ttu-id="20a48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20a48-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20a48-108">Permission type</span></span>                        | <span data-ttu-id="20a48-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20a48-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20a48-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20a48-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="20a48-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="20a48-111">Policy.Read.All</span></span> |
| <span data-ttu-id="20a48-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20a48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20a48-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20a48-113">Not supported.</span></span> |
| <span data-ttu-id="20a48-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20a48-114">Application</span></span>                            | <span data-ttu-id="20a48-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="20a48-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20a48-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20a48-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20a48-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20a48-117">Optional query parameters</span></span>

<span data-ttu-id="20a48-118">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="20a48-118">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="20a48-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="20a48-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="20a48-120">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="20a48-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20a48-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20a48-121">Request headers</span></span>

| <span data-ttu-id="20a48-122">Имя</span><span class="sxs-lookup"><span data-stu-id="20a48-122">Name</span></span>      |<span data-ttu-id="20a48-123">Описание</span><span class="sxs-lookup"><span data-stu-id="20a48-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20a48-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20a48-124">Authorization</span></span> | <span data-ttu-id="20a48-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="20a48-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="20a48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20a48-126">Request body</span></span>

<span data-ttu-id="20a48-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20a48-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20a48-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="20a48-128">Response</span></span>

<span data-ttu-id="20a48-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20a48-129">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20a48-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="20a48-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20a48-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="20a48-131">Request</span></span>

<span data-ttu-id="20a48-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20a48-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="20a48-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="20a48-133">Response</span></span>

<span data-ttu-id="20a48-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="20a48-134">The following is an example of the response.</span></span>

> <span data-ttu-id="20a48-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20a48-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->