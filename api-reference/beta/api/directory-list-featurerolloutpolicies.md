---
title: Список ФеатурероллаутполиЦиес
description: Получение списка объектов Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 782771ab560101996182099ace532dc08f41b10f
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062166"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="8c377-103">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="8c377-103">List featureRolloutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c377-104">Получение списка объектов [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8c377-104">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c377-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c377-105">Permissions</span></span>

<span data-ttu-id="8c377-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c377-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c377-108">Permission type</span></span>                        | <span data-ttu-id="8c377-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c377-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c377-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c377-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c377-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c377-111">Policy.Read.All</span></span> |
| <span data-ttu-id="8c377-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c377-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c377-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c377-113">Not supported.</span></span> |
| <span data-ttu-id="8c377-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c377-114">Application</span></span>                            | <span data-ttu-id="8c377-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c377-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c377-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c377-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c377-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c377-117">Optional query parameters</span></span>

<span data-ttu-id="8c377-118">Этот метод поддерживает следующие параметры `$count`запроса OData для настройки отклика:, `$expand` `$filter` `$orderby` `$select`,,,, `$skip`,. `$top`</span><span class="sxs-lookup"><span data-stu-id="8c377-118">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="8c377-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c377-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c377-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c377-120">Request headers</span></span>

| <span data-ttu-id="8c377-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8c377-121">Name</span></span>      |<span data-ttu-id="8c377-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c377-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c377-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c377-123">Authorization</span></span> | <span data-ttu-id="8c377-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8c377-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c377-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c377-125">Request body</span></span>

<span data-ttu-id="8c377-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c377-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c377-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c377-127">Response</span></span>

<span data-ttu-id="8c377-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c377-128">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c377-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c377-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c377-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c377-130">Request</span></span>

<span data-ttu-id="8c377-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c377-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```

### <a name="response"></a><span data-ttu-id="8c377-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c377-132">Response</span></span>

<span data-ttu-id="8c377-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c377-133">The following is an example of the response.</span></span>

> <span data-ttu-id="8c377-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c377-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
