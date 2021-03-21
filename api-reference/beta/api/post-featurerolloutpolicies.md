---
title: Создание featureRolloutPolicy
description: Создайте новый объект featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bd14edf1a50d26e947af11eaf1239695b7aeb214
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965250"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="c2986-103">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="c2986-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="c2986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2986-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2986-105">Создайте новый [объект featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c2986-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2986-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2986-106">Permissions</span></span>

<span data-ttu-id="c2986-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2986-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2986-109">Permission type</span></span>                        | <span data-ttu-id="c2986-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2986-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2986-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2986-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2986-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2986-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c2986-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2986-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2986-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2986-114">Not supported.</span></span> |
| <span data-ttu-id="c2986-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2986-115">Application</span></span>                            | <span data-ttu-id="c2986-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2986-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2986-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2986-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c2986-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2986-118">Request headers</span></span>

| <span data-ttu-id="c2986-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c2986-119">Name</span></span>          | <span data-ttu-id="c2986-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c2986-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2986-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2986-121">Authorization</span></span> | <span data-ttu-id="c2986-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c2986-122">Bearer {token}.</span></span> <span data-ttu-id="c2986-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c2986-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2986-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2986-124">Request body</span></span>

<span data-ttu-id="c2986-125">В теле запроса поставляем представление JSON объекта [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c2986-125">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="c2986-126">В следующей таблице показаны свойства, необходимые при создании [featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c2986-126">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="c2986-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2986-127">Parameter</span></span> | <span data-ttu-id="c2986-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c2986-128">Type</span></span> | <span data-ttu-id="c2986-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2986-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2986-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c2986-130">displayName</span></span> |<span data-ttu-id="c2986-131">string</span><span class="sxs-lookup"><span data-stu-id="c2986-131">string</span></span> |<span data-ttu-id="c2986-132">Имя отображения для этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="c2986-132">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="c2986-133">функция</span><span class="sxs-lookup"><span data-stu-id="c2986-133">feature</span></span> |<span data-ttu-id="c2986-134">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="c2986-134">stagedFeatureName</span></span> |<span data-ttu-id="c2986-135">Функция, которая будет выкатываться с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="c2986-135">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="c2986-136">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c2986-136">isEnabled</span></span> |<span data-ttu-id="c2986-137">string</span><span class="sxs-lookup"><span data-stu-id="c2986-137">string</span></span> |<span data-ttu-id="c2986-138">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="c2986-138">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="c2986-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2986-139">Response</span></span>

<span data-ttu-id="c2986-140">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2986-140">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2986-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2986-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2986-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2986-142">Request</span></span>

<span data-ttu-id="c2986-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2986-143">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="c2986-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2986-144">Response</span></span>

<span data-ttu-id="c2986-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2986-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c2986-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2986-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


