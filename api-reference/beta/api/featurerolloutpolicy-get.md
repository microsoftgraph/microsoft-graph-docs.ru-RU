---
title: Получение Феатурероллаутполици
description: Получение свойств и связей объекта феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c36c8db23e0550ac1d68aea363ce7921d82a3a0
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062172"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="18653-103">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="18653-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18653-104">Получение свойств и связей объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="18653-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18653-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18653-105">Permissions</span></span>

<span data-ttu-id="18653-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18653-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18653-108">Permission type</span></span>                        | <span data-ttu-id="18653-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18653-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18653-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18653-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="18653-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="18653-111">Policy.Read.All</span></span> |
| <span data-ttu-id="18653-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18653-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18653-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18653-113">Not supported.</span></span> |
| <span data-ttu-id="18653-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18653-114">Application</span></span>                            | <span data-ttu-id="18653-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18653-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18653-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18653-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18653-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18653-117">Optional query parameters</span></span>

<span data-ttu-id="18653-118">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18653-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="18653-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="18653-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="18653-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18653-120">Request headers</span></span>

| <span data-ttu-id="18653-121">Имя</span><span class="sxs-lookup"><span data-stu-id="18653-121">Name</span></span>      |<span data-ttu-id="18653-122">Описание</span><span class="sxs-lookup"><span data-stu-id="18653-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18653-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18653-123">Authorization</span></span> | <span data-ttu-id="18653-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="18653-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="18653-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18653-125">Request body</span></span>

<span data-ttu-id="18653-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18653-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18653-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="18653-127">Response</span></span>

<span data-ttu-id="18653-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18653-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18653-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="18653-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18653-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="18653-130">Request</span></span>

<span data-ttu-id="18653-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18653-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="18653-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="18653-132">Response</span></span>

<span data-ttu-id="18653-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18653-133">The following is an example of the response.</span></span>

> <span data-ttu-id="18653-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18653-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="18653-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="18653-136">Request</span></span>

<span data-ttu-id="18653-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18653-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

### <a name="response"></a><span data-ttu-id="18653-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="18653-138">Response</span></span>

<span data-ttu-id="18653-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18653-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="18653-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18653-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18653-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18653-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
