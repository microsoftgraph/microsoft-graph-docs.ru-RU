---
title: Создание featureRolloutPolicy
description: Создайте новый объект featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1ec54a67867ecbf62da04fc87c6f1e7b9d043755
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436969"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="12fc0-103">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="12fc0-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="12fc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12fc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12fc0-105">Создайте новый [объект featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12fc0-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12fc0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc0-106">Permissions</span></span>

<span data-ttu-id="12fc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12fc0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc0-109">Permission type</span></span>                        | <span data-ttu-id="12fc0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fc0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="12fc0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fc0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12fc0-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="12fc0-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="12fc0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fc0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc0-114">Not supported.</span></span> |
| <span data-ttu-id="12fc0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fc0-115">Application</span></span>                            | <span data-ttu-id="12fc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12fc0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="12fc0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fc0-118">Request headers</span></span>

| <span data-ttu-id="12fc0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="12fc0-119">Name</span></span>          | <span data-ttu-id="12fc0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="12fc0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="12fc0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12fc0-121">Authorization</span></span> | <span data-ttu-id="12fc0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="12fc0-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="12fc0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12fc0-123">Request body</span></span>

<span data-ttu-id="12fc0-124">В теле запроса поставляем представление JSON объекта [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12fc0-124">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="12fc0-125">В следующей таблице показаны свойства, необходимые при создании [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12fc0-125">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="12fc0-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="12fc0-126">Parameter</span></span> | <span data-ttu-id="12fc0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="12fc0-127">Type</span></span> | <span data-ttu-id="12fc0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="12fc0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12fc0-129">displayName</span><span class="sxs-lookup"><span data-stu-id="12fc0-129">displayName</span></span> |<span data-ttu-id="12fc0-130">string</span><span class="sxs-lookup"><span data-stu-id="12fc0-130">string</span></span> |<span data-ttu-id="12fc0-131">Имя отображения для этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="12fc0-131">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="12fc0-132">функция</span><span class="sxs-lookup"><span data-stu-id="12fc0-132">feature</span></span> |<span data-ttu-id="12fc0-133">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="12fc0-133">stagedFeatureName</span></span> |<span data-ttu-id="12fc0-134">Функция, которая будет выкатываться с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="12fc0-134">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="12fc0-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="12fc0-135">isEnabled</span></span> |<span data-ttu-id="12fc0-136">string</span><span class="sxs-lookup"><span data-stu-id="12fc0-136">string</span></span> |<span data-ttu-id="12fc0-137">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="12fc0-137">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="12fc0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc0-138">Response</span></span>

<span data-ttu-id="12fc0-139">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="12fc0-139">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12fc0-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="12fc0-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12fc0-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fc0-141">Request</span></span>

<span data-ttu-id="12fc0-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fc0-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12fc0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="12fc0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="12fc0-144">C#</span><span class="sxs-lookup"><span data-stu-id="12fc0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12fc0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12fc0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12fc0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12fc0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12fc0-147">Java</span><span class="sxs-lookup"><span data-stu-id="12fc0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12fc0-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc0-148">Response</span></span>

<span data-ttu-id="12fc0-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fc0-149">The following is an example of the response.</span></span>

> <span data-ttu-id="12fc0-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12fc0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


