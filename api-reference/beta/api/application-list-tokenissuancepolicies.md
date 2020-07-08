---
title: Список назначенных ТокениссуанцеполиЦиес
description: Список ТокениссуанцеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99e6811d3462afd64548063685e20225459d0f3a
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081300"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="cca65-103">Список назначенных ТокениссуанцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="cca65-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="cca65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cca65-105">Перечисление объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="cca65-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cca65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cca65-106">Permissions</span></span>

<span data-ttu-id="cca65-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cca65-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cca65-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cca65-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cca65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cca65-109">Permission type</span></span>                        | <span data-ttu-id="cca65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cca65-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cca65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cca65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cca65-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cca65-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="cca65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cca65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cca65-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cca65-114">Not supported.</span></span> |
| <span data-ttu-id="cca65-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cca65-115">Application</span></span>                            | <span data-ttu-id="cca65-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cca65-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cca65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cca65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cca65-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cca65-118">Request headers</span></span>

| <span data-ttu-id="cca65-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cca65-119">Name</span></span>          | <span data-ttu-id="cca65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cca65-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cca65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cca65-121">Authorization</span></span> | <span data-ttu-id="cca65-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="cca65-122">Bearer {token}.</span></span> <span data-ttu-id="cca65-123">Required.</span><span class="sxs-lookup"><span data-stu-id="cca65-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cca65-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cca65-124">Request body</span></span>

<span data-ttu-id="cca65-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cca65-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cca65-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca65-126">Response</span></span>

<span data-ttu-id="cca65-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cca65-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cca65-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cca65-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cca65-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cca65-129">Request</span></span>

<span data-ttu-id="cca65-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cca65-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cca65-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cca65-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="cca65-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="cca65-132">Response</span></span>

<span data-ttu-id="cca65-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cca65-133">The following is an example of the response.</span></span>

> <span data-ttu-id="cca65-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="cca65-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cca65-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cca65-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
