---
title: Удаление featureRolloutPolicy
description: Удаление объекта featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ac2d8f8acba29db911030718fbb37e4ddfe53093
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955933"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="503d3-103">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="503d3-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="503d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="503d3-105">Удаление [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="503d3-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="503d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="503d3-106">Permissions</span></span>

<span data-ttu-id="503d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="503d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="503d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="503d3-109">Permission type</span></span>                        | <span data-ttu-id="503d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="503d3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="503d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="503d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="503d3-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="503d3-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="503d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="503d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="503d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503d3-114">Not supported.</span></span> |
| <span data-ttu-id="503d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="503d3-115">Application</span></span>                            | <span data-ttu-id="503d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503d3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="503d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="503d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="503d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="503d3-118">Request headers</span></span>

| <span data-ttu-id="503d3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="503d3-119">Name</span></span>          | <span data-ttu-id="503d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="503d3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="503d3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="503d3-121">Authorization</span></span> | <span data-ttu-id="503d3-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="503d3-122">Bearer {token}.</span></span> <span data-ttu-id="503d3-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="503d3-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="503d3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="503d3-124">Request body</span></span>

<span data-ttu-id="503d3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="503d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="503d3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="503d3-126">Response</span></span>

<span data-ttu-id="503d3-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="503d3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="503d3-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="503d3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="503d3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="503d3-130">Request</span></span>

<span data-ttu-id="503d3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="503d3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="503d3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="503d3-132">Response</span></span>

<span data-ttu-id="503d3-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="503d3-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


