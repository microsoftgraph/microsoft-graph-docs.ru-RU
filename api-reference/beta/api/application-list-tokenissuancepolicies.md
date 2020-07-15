---
title: Список назначенных ТокениссуанцеполиЦиес
description: Список ТокениссуанцеполиЦиес, назначенных приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c39d82332e2ea278afd169f059e642c66c59bdc
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142289"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="bdd8d-103">Список назначенных ТокениссуанцеполиЦиес</span><span class="sxs-lookup"><span data-stu-id="bdd8d-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="bdd8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd8d-105">Перечисление объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) , назначенных [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="bdd8d-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd8d-106">Permissions</span></span>

<span data-ttu-id="bdd8d-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bdd8d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd8d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdd8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdd8d-109">Permission type</span></span>                        | <span data-ttu-id="bdd8d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdd8d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdd8d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdd8d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdd8d-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bdd8d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="bdd8d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdd8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd8d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-114">Not supported.</span></span> |
| <span data-ttu-id="bdd8d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="bdd8d-115">Application</span></span>                            | <span data-ttu-id="bdd8d-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bdd8d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd8d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdd8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bdd8d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdd8d-118">Request headers</span></span>

| <span data-ttu-id="bdd8d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bdd8d-119">Name</span></span>          | <span data-ttu-id="bdd8d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bdd8d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bdd8d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdd8d-121">Authorization</span></span> | <span data-ttu-id="bdd8d-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-122">Bearer {token}.</span></span> <span data-ttu-id="bdd8d-123">Required.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd8d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bdd8d-124">Request body</span></span>

<span data-ttu-id="bdd8d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdd8d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd8d-126">Response</span></span>

<span data-ttu-id="bdd8d-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токениссуанцеполици](../resources/tokenissuancepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdd8d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="bdd8d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdd8d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdd8d-129">Request</span></span>

<span data-ttu-id="bdd8d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bdd8d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd8d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="bdd8d-132">C#</span><span class="sxs-lookup"><span data-stu-id="bdd8d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdd8d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdd8d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdd8d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdd8d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bdd8d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdd8d-135">Response</span></span>

<span data-ttu-id="bdd8d-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-136">The following is an example of the response.</span></span>

> <span data-ttu-id="bdd8d-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bdd8d-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bdd8d-138">All the properties will be returned from an actual call.</span></span>

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
