---
title: Создание featureRolloutPolicy
description: Создайте новый объект featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 020513c2eb1fdc8b05d49b1f34979dcfecf17623
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049921"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="4b28b-103">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="4b28b-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="4b28b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b28b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b28b-105">Создайте новый [объект featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b28b-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b28b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b28b-106">Permissions</span></span>

<span data-ttu-id="4b28b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b28b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b28b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b28b-109">Permission type</span></span>                        | <span data-ttu-id="4b28b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b28b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b28b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b28b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b28b-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b28b-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="4b28b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b28b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b28b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b28b-114">Not supported.</span></span> |
| <span data-ttu-id="4b28b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b28b-115">Application</span></span>                            | <span data-ttu-id="4b28b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b28b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b28b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b28b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4b28b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b28b-118">Request headers</span></span>

| <span data-ttu-id="4b28b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4b28b-119">Name</span></span>          | <span data-ttu-id="4b28b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4b28b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b28b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b28b-121">Authorization</span></span> | <span data-ttu-id="4b28b-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4b28b-122">Bearer {token}.</span></span> <span data-ttu-id="4b28b-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="4b28b-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b28b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b28b-124">Request body</span></span>

<span data-ttu-id="4b28b-125">В теле запроса поставляем представление JSON объекта [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b28b-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="4b28b-126">В следующей таблице показаны свойства, необходимые при создании [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4b28b-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="4b28b-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b28b-127">Parameter</span></span> | <span data-ttu-id="4b28b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4b28b-128">Type</span></span> | <span data-ttu-id="4b28b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4b28b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b28b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4b28b-130">displayName</span></span> |<span data-ttu-id="4b28b-131">string</span><span class="sxs-lookup"><span data-stu-id="4b28b-131">string</span></span> |<span data-ttu-id="4b28b-132">Имя отображения для этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="4b28b-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="4b28b-133">функция</span><span class="sxs-lookup"><span data-stu-id="4b28b-133">feature</span></span> |<span data-ttu-id="4b28b-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="4b28b-134">stagedFeatureName</span></span> |<span data-ttu-id="4b28b-135">Функция, которая будет выкатываться с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b28b-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="4b28b-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4b28b-136">isEnabled</span></span> |<span data-ttu-id="4b28b-137">String</span><span class="sxs-lookup"><span data-stu-id="4b28b-137">string</span></span> |<span data-ttu-id="4b28b-138">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="4b28b-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="4b28b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b28b-139">Response</span></span>

<span data-ttu-id="4b28b-140">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4b28b-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b28b-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b28b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b28b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b28b-142">Request</span></span>

<span data-ttu-id="4b28b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b28b-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b28b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b28b-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4b28b-145">C#</span><span class="sxs-lookup"><span data-stu-id="4b28b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b28b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b28b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b28b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b28b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b28b-148">Java</span><span class="sxs-lookup"><span data-stu-id="4b28b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b28b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b28b-149">Response</span></span>

<span data-ttu-id="4b28b-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b28b-150">The following is an example of the response.</span></span>

> <span data-ttu-id="4b28b-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b28b-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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


