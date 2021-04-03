---
title: Функция ListRolloutPolicies
description: Извлечение списка объектов featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e64cf90e3d5fd78fb8515fe72dbcfd7bd889ab01
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509149"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="5fa95-103">Функция ListRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="5fa95-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="5fa95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fa95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fa95-105">Извлечение списка [объектов featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fa95-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fa95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fa95-106">Permissions</span></span>

<span data-ttu-id="5fa95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fa95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fa95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fa95-109">Permission type</span></span>                        | <span data-ttu-id="5fa95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fa95-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5fa95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fa95-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fa95-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fa95-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="5fa95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fa95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fa95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fa95-114">Not supported.</span></span> |
| <span data-ttu-id="5fa95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fa95-115">Application</span></span>                            | <span data-ttu-id="5fa95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fa95-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fa95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fa95-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fa95-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5fa95-118">Optional query parameters</span></span>

<span data-ttu-id="5fa95-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ: `$count` , , , , , , `$expand` `$filter` `$orderby` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5fa95-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="5fa95-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5fa95-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fa95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fa95-121">Request headers</span></span>

| <span data-ttu-id="5fa95-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5fa95-122">Name</span></span>      |<span data-ttu-id="5fa95-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5fa95-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fa95-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fa95-124">Authorization</span></span> | <span data-ttu-id="5fa95-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5fa95-125">Bearer {token}.</span></span> <span data-ttu-id="5fa95-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="5fa95-126">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fa95-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fa95-127">Request body</span></span>

<span data-ttu-id="5fa95-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5fa95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fa95-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fa95-129">Response</span></span>

<span data-ttu-id="5fa95-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [featureRolloutPolicy](../resources/featurerolloutpolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5fa95-130">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fa95-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5fa95-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fa95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fa95-132">Request</span></span>

<span data-ttu-id="5fa95-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fa95-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5fa95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fa95-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="5fa95-135">C#</span><span class="sxs-lookup"><span data-stu-id="5fa95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fa95-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fa95-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fa95-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fa95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fa95-138">Java</span><span class="sxs-lookup"><span data-stu-id="5fa95-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicies-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5fa95-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fa95-139">Response</span></span>

<span data-ttu-id="5fa95-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5fa95-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5fa95-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5fa95-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


