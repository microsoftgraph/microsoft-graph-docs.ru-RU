---
title: Обновление функцииRolloutPolicy
description: Обновление свойств объекта featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 66b04005f01f9e2d56189a23ad8dae36846a67a0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787002"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="f2f6e-103">Обновление featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="f2f6e-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="f2f6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2f6e-105">Обновление свойств [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2f6e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f6e-106">Permissions</span></span>

<span data-ttu-id="f2f6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2f6e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f6e-109">Permission type</span></span>                        | <span data-ttu-id="f2f6e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f2f6e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2f6e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f6e-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f2f6e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f6e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-114">Not supported.</span></span> |
| <span data-ttu-id="f2f6e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2f6e-115">Application</span></span>                            | <span data-ttu-id="f2f6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f6e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2f6e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f2f6e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2f6e-118">Request headers</span></span>

| <span data-ttu-id="f2f6e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f2f6e-119">Name</span></span>       | <span data-ttu-id="f2f6e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f6e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f2f6e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2f6e-121">Authorization</span></span> | <span data-ttu-id="f2f6e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-122">Bearer {token}.</span></span> <span data-ttu-id="f2f6e-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f2f6e-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2f6e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2f6e-124">Request body</span></span>

<span data-ttu-id="f2f6e-125">В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-125">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="f2f6e-126">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-126">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="f2f6e-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f2f6e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2f6e-128">Property</span></span>     | <span data-ttu-id="f2f6e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f2f6e-129">Type</span></span>        | <span data-ttu-id="f2f6e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f6e-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2f6e-131">description</span><span class="sxs-lookup"><span data-stu-id="f2f6e-131">description</span></span>|<span data-ttu-id="f2f6e-132">String</span><span class="sxs-lookup"><span data-stu-id="f2f6e-132">String</span></span>|<span data-ttu-id="f2f6e-133">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-133">A description for this policy.</span></span>|
|<span data-ttu-id="f2f6e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f2f6e-134">displayName</span></span>|<span data-ttu-id="f2f6e-135">String</span><span class="sxs-lookup"><span data-stu-id="f2f6e-135">String</span></span>|<span data-ttu-id="f2f6e-136">Имя отображения для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-136">The display name for this policy.</span></span>|
|<span data-ttu-id="f2f6e-137">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="f2f6e-137">isAppliedToOrganization</span></span>|<span data-ttu-id="f2f6e-138">Логический</span><span class="sxs-lookup"><span data-stu-id="f2f6e-138">Boolean</span></span>|<span data-ttu-id="f2f6e-139">Указывает, следует ли применять эту политику выкатки функций ко всей организации.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-139">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="f2f6e-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f2f6e-140">isEnabled</span></span>|<span data-ttu-id="f2f6e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2f6e-141">Boolean</span></span>|<span data-ttu-id="f2f6e-142">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-142">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="f2f6e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f6e-143">Response</span></span>

<span data-ttu-id="f2f6e-144">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-144">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2f6e-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2f6e-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2f6e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2f6e-146">Request</span></span>

<span data-ttu-id="f2f6e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2f6e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f6e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy_policies"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```
# <a name="c"></a>[<span data-ttu-id="f2f6e-149">C#</span><span class="sxs-lookup"><span data-stu-id="f2f6e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2f6e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2f6e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2f6e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2f6e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2f6e-152">Java</span><span class="sxs-lookup"><span data-stu-id="f2f6e-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2f6e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f6e-153">Response</span></span>

<span data-ttu-id="f2f6e-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


