---
title: Обновление функцииRolloutPolicy
description: Обновление свойств объекта featurerolloutpolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3604a9a3acd64988e68811076e671d9905d874fb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964880"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="368cb-103">Обновление featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="368cb-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="368cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="368cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="368cb-105">Обновление свойств [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="368cb-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="368cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="368cb-106">Permissions</span></span>

<span data-ttu-id="368cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="368cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="368cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="368cb-109">Permission type</span></span>                        | <span data-ttu-id="368cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="368cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="368cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="368cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="368cb-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="368cb-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="368cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="368cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="368cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="368cb-114">Not supported.</span></span> |
| <span data-ttu-id="368cb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="368cb-115">Application</span></span>                            | <span data-ttu-id="368cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="368cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="368cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="368cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="368cb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="368cb-118">Request headers</span></span>

| <span data-ttu-id="368cb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="368cb-119">Name</span></span>       | <span data-ttu-id="368cb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="368cb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="368cb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="368cb-121">Authorization</span></span> | <span data-ttu-id="368cb-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="368cb-122">Bearer {token}.</span></span> <span data-ttu-id="368cb-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="368cb-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="368cb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="368cb-124">Request body</span></span>

<span data-ttu-id="368cb-125">В теле запроса укажи значения для соответствующих свойств, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="368cb-125">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="368cb-126">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="368cb-126">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="368cb-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="368cb-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="368cb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="368cb-128">Property</span></span>     | <span data-ttu-id="368cb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="368cb-129">Type</span></span>        | <span data-ttu-id="368cb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="368cb-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="368cb-131">description</span><span class="sxs-lookup"><span data-stu-id="368cb-131">description</span></span>|<span data-ttu-id="368cb-132">String</span><span class="sxs-lookup"><span data-stu-id="368cb-132">String</span></span>|<span data-ttu-id="368cb-133">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="368cb-133">A description for this policy.</span></span>|
|<span data-ttu-id="368cb-134">displayName</span><span class="sxs-lookup"><span data-stu-id="368cb-134">displayName</span></span>|<span data-ttu-id="368cb-135">String</span><span class="sxs-lookup"><span data-stu-id="368cb-135">String</span></span>|<span data-ttu-id="368cb-136">Имя отображения для этой политики.</span><span class="sxs-lookup"><span data-stu-id="368cb-136">The display name for this policy.</span></span>|
|<span data-ttu-id="368cb-137">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="368cb-137">isAppliedToOrganization</span></span>|<span data-ttu-id="368cb-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="368cb-138">Boolean</span></span>|<span data-ttu-id="368cb-139">Указывает, следует ли применять эту политику выкатки функций ко всей организации.</span><span class="sxs-lookup"><span data-stu-id="368cb-139">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="368cb-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="368cb-140">isEnabled</span></span>|<span data-ttu-id="368cb-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="368cb-141">Boolean</span></span>|<span data-ttu-id="368cb-142">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="368cb-142">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="368cb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="368cb-143">Response</span></span>

<span data-ttu-id="368cb-144">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="368cb-144">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="368cb-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="368cb-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="368cb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="368cb-146">Request</span></span>

<span data-ttu-id="368cb-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="368cb-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a
Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="368cb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="368cb-148">Response</span></span>

<span data-ttu-id="368cb-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="368cb-149">The following is an example of the response.</span></span>

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


