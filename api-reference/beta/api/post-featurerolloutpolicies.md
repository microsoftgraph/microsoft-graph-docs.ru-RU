---
title: Создание featureRolloutPolicy
description: Создайте новый объект featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b731778c096470f23799540919ff93f9a8e52853
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508357"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="c82e9-103">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c82e9-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="c82e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c82e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c82e9-105">Создайте новый [объект featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c82e9-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c82e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c82e9-106">Permissions</span></span>

<span data-ttu-id="c82e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c82e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c82e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c82e9-109">Permission type</span></span>                        | <span data-ttu-id="c82e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c82e9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c82e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c82e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c82e9-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82e9-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c82e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c82e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c82e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c82e9-114">Not supported.</span></span> |
| <span data-ttu-id="c82e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c82e9-115">Application</span></span>                            | <span data-ttu-id="c82e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c82e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c82e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c82e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c82e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c82e9-118">Request headers</span></span>

| <span data-ttu-id="c82e9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c82e9-119">Name</span></span>          | <span data-ttu-id="c82e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c82e9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c82e9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c82e9-121">Authorization</span></span> | <span data-ttu-id="c82e9-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c82e9-122">Bearer {token}.</span></span> <span data-ttu-id="c82e9-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="c82e9-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="c82e9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c82e9-124">Request body</span></span>

<span data-ttu-id="c82e9-125">В теле запроса поставляем представление JSON объекта [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c82e9-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="c82e9-126">В следующей таблице показаны свойства, необходимые при создании [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c82e9-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="c82e9-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="c82e9-127">Parameter</span></span> | <span data-ttu-id="c82e9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c82e9-128">Type</span></span> | <span data-ttu-id="c82e9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c82e9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c82e9-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c82e9-130">displayName</span></span> |<span data-ttu-id="c82e9-131">string</span><span class="sxs-lookup"><span data-stu-id="c82e9-131">string</span></span> |<span data-ttu-id="c82e9-132">Имя отображения для этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="c82e9-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="c82e9-133">функция</span><span class="sxs-lookup"><span data-stu-id="c82e9-133">feature</span></span> |<span data-ttu-id="c82e9-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="c82e9-134">stagedFeatureName</span></span> |<span data-ttu-id="c82e9-135">Функция, которая будет выкатываться с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="c82e9-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="c82e9-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c82e9-136">isEnabled</span></span> |<span data-ttu-id="c82e9-137">string</span><span class="sxs-lookup"><span data-stu-id="c82e9-137">string</span></span> |<span data-ttu-id="c82e9-138">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="c82e9-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="c82e9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82e9-139">Response</span></span>

<span data-ttu-id="c82e9-140">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c82e9-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c82e9-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="c82e9-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c82e9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c82e9-142">Request</span></span>

<span data-ttu-id="c82e9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c82e9-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c82e9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c82e9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_policies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="c82e9-145">C#</span><span class="sxs-lookup"><span data-stu-id="c82e9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c82e9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c82e9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c82e9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c82e9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c82e9-148">Java</span><span class="sxs-lookup"><span data-stu-id="c82e9-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c82e9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82e9-149">Response</span></span>

<span data-ttu-id="c82e9-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c82e9-150">The following is an example of the response.</span></span>

> <span data-ttu-id="c82e9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c82e9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


