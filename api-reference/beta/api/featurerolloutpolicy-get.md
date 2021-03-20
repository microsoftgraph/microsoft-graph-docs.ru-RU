---
title: Get featureRolloutPolicy
description: Извлечение свойств и связей объекта featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 956f5cada595471a1e9425b1399c69b4f4bc728c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955926"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="b8f82-103">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="b8f82-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="b8f82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8f82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8f82-105">Извлечение свойств и связей [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b8f82-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8f82-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8f82-106">Permissions</span></span>

<span data-ttu-id="b8f82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8f82-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8f82-109">Permission type</span></span>                        | <span data-ttu-id="b8f82-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8f82-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8f82-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8f82-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8f82-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8f82-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b8f82-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8f82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8f82-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8f82-114">Not supported.</span></span> |
| <span data-ttu-id="b8f82-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8f82-115">Application</span></span>                            | <span data-ttu-id="b8f82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8f82-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8f82-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8f82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8f82-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8f82-118">Optional query parameters</span></span>

<span data-ttu-id="b8f82-119">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b8f82-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="b8f82-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b8f82-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8f82-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8f82-121">Request headers</span></span>

| <span data-ttu-id="b8f82-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b8f82-122">Name</span></span>      |<span data-ttu-id="b8f82-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b8f82-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8f82-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8f82-124">Authorization</span></span> | <span data-ttu-id="b8f82-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b8f82-125">Bearer {token}.</span></span> <span data-ttu-id="b8f82-126">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b8f82-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8f82-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8f82-127">Request body</span></span>

<span data-ttu-id="b8f82-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8f82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f82-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8f82-129">Response</span></span>

<span data-ttu-id="b8f82-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8f82-130">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8f82-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b8f82-131">Examples</span></span>

### <a name="example-1-get-a-feature-rollout-policy"></a><span data-ttu-id="b8f82-132">Пример 1. Получить политику выкатки функций</span><span class="sxs-lookup"><span data-stu-id="b8f82-132">Example 1: Get a feature rollout policy</span></span>

#### <a name="request"></a><span data-ttu-id="b8f82-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8f82-133">Request</span></span>

<span data-ttu-id="b8f82-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8f82-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
#### <a name="response"></a><span data-ttu-id="b8f82-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8f82-135">Response</span></span>

<span data-ttu-id="b8f82-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8f82-136">The following is an example of the response.</span></span>

> <span data-ttu-id="b8f82-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8f82-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-feature-rollout-policy-and-expand-appliesto"></a><span data-ttu-id="b8f82-139">Пример 2. Получить политику выкатки функций и расширить appliesTo</span><span class="sxs-lookup"><span data-stu-id="b8f82-139">Example 2: Get a feature rollout policy and expand appliesTo</span></span>

#### <a name="request"></a><span data-ttu-id="b8f82-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8f82-140">Request</span></span>

<span data-ttu-id="b8f82-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8f82-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy_expandAppliesTo_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```

#### <a name="response"></a><span data-ttu-id="b8f82-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8f82-142">Response</span></span>

<span data-ttu-id="b8f82-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b8f82-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b8f82-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b8f82-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


