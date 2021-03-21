---
title: Обновление функцииRolloutPolicy
description: Обновление свойств объекта featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 91567639b46a369305e8b02a3ee4cdde77f21aad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959272"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="770e3-103">Обновление featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="770e3-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="770e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="770e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="770e3-105">Обновление свойств [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="770e3-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="770e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="770e3-106">Permissions</span></span>

<span data-ttu-id="770e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="770e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="770e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="770e3-109">Permission type</span></span>                        | <span data-ttu-id="770e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="770e3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="770e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="770e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="770e3-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770e3-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="770e3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="770e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="770e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="770e3-114">Not supported.</span></span> |
| <span data-ttu-id="770e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="770e3-115">Application</span></span>                            | <span data-ttu-id="770e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="770e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="770e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="770e3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="770e3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="770e3-118">Request headers</span></span>

| <span data-ttu-id="770e3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="770e3-119">Name</span></span>       | <span data-ttu-id="770e3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="770e3-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="770e3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="770e3-121">Authorization</span></span> | <span data-ttu-id="770e3-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="770e3-122">Bearer {token}.</span></span> <span data-ttu-id="770e3-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="770e3-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="770e3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="770e3-124">Request body</span></span>

<span data-ttu-id="770e3-125">В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="770e3-125">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="770e3-126">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="770e3-126">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="770e3-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="770e3-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="770e3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="770e3-128">Property</span></span>     | <span data-ttu-id="770e3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="770e3-129">Type</span></span>        | <span data-ttu-id="770e3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="770e3-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="770e3-131">description</span><span class="sxs-lookup"><span data-stu-id="770e3-131">description</span></span>|<span data-ttu-id="770e3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="770e3-132">String</span></span>|<span data-ttu-id="770e3-133">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="770e3-133">A description for this policy.</span></span>|
|<span data-ttu-id="770e3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="770e3-134">displayName</span></span>|<span data-ttu-id="770e3-135">Строка</span><span class="sxs-lookup"><span data-stu-id="770e3-135">String</span></span>|<span data-ttu-id="770e3-136">Имя отображения для этой политики.</span><span class="sxs-lookup"><span data-stu-id="770e3-136">The display name for this policy.</span></span>|
|<span data-ttu-id="770e3-137">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="770e3-137">isAppliedToOrganization</span></span>|<span data-ttu-id="770e3-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="770e3-138">Boolean</span></span>|<span data-ttu-id="770e3-139">Указывает, следует ли применять эту политику выкатки функций ко всей организации.</span><span class="sxs-lookup"><span data-stu-id="770e3-139">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="770e3-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="770e3-140">isEnabled</span></span>|<span data-ttu-id="770e3-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="770e3-141">Boolean</span></span>|<span data-ttu-id="770e3-142">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="770e3-142">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="770e3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="770e3-143">Response</span></span>

<span data-ttu-id="770e3-144">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="770e3-144">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="770e3-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="770e3-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="770e3-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="770e3-146">Request</span></span>

<span data-ttu-id="770e3-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="770e3-147">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="770e3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="770e3-148">Response</span></span>

<span data-ttu-id="770e3-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="770e3-149">The following is an example of the response.</span></span>

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
  "description": "Update featurerolloutpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


