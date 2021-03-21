---
title: Удаление appliesTo
description: Удалите directoryObject из выкатки функций.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 04327bd52f34de054bbb5451ed4c53a3695afa34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955947"
---
# <a name="remove-appliesto"></a><span data-ttu-id="caf4e-103">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="caf4e-103">Remove appliesTo</span></span>

<span data-ttu-id="caf4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caf4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caf4e-105">Удалите appliesTo на [объекте featureRolloutPolicy,](../resources/featurerolloutpolicy.md) чтобы удалить [directoryObject](../resources/directoryobject.md) из выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="caf4e-105">Remove an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to remove the [directoryObject](../resources/directoryobject.md) from feature rollout.</span></span>

## <a name="permissions"></a><span data-ttu-id="caf4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="caf4e-106">Permissions</span></span>

<span data-ttu-id="caf4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caf4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="caf4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="caf4e-109">Permission type</span></span>                        | <span data-ttu-id="caf4e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="caf4e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="caf4e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="caf4e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="caf4e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caf4e-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="caf4e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="caf4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caf4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf4e-114">Not supported.</span></span> |
| <span data-ttu-id="caf4e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="caf4e-115">Application</span></span>                            | <span data-ttu-id="caf4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="caf4e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="caf4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="caf4e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{policyId}/appliesTo/{directoryObjectId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="caf4e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="caf4e-118">Request headers</span></span>

| <span data-ttu-id="caf4e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="caf4e-119">Name</span></span>          | <span data-ttu-id="caf4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="caf4e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="caf4e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="caf4e-121">Authorization</span></span> | <span data-ttu-id="caf4e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="caf4e-122">Bearer {token}.</span></span> <span data-ttu-id="caf4e-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="caf4e-123">Required</span></span> |

## <a name="response"></a><span data-ttu-id="caf4e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf4e-124">Response</span></span>

<span data-ttu-id="caf4e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="caf4e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="caf4e-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="caf4e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="caf4e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="caf4e-128">Request</span></span>

<span data-ttu-id="caf4e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="caf4e-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref
```

### <a name="response"></a><span data-ttu-id="caf4e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="caf4e-130">Response</span></span>

<span data-ttu-id="caf4e-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="caf4e-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


