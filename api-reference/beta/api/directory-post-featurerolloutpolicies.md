---
title: Создание Феатурероллаутполици
description: Создание нового объекта Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc2ed04abef450415cc4ee9802cceed687dc324b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435201"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="0ea21-103">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="0ea21-103">Create featureRolloutPolicy</span></span>

<span data-ttu-id="0ea21-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ea21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea21-105">Создание нового объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0ea21-105">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea21-106">Permissions</span></span>

<span data-ttu-id="0ea21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ea21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea21-109">Permission type</span></span>                        | <span data-ttu-id="0ea21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ea21-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ea21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ea21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ea21-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="0ea21-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="0ea21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ea21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea21-114">Not supported.</span></span> |
| <span data-ttu-id="0ea21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ea21-115">Application</span></span>                            | <span data-ttu-id="0ea21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea21-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ea21-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0ea21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ea21-118">Request headers</span></span>

| <span data-ttu-id="0ea21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ea21-119">Name</span></span>          | <span data-ttu-id="0ea21-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea21-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0ea21-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ea21-121">Authorization</span></span> | <span data-ttu-id="0ea21-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ea21-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea21-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ea21-123">Request body</span></span>

<span data-ttu-id="0ea21-124">В тексте запроса добавьте представление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ea21-124">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="0ea21-125">В следующей таблице приведены свойства, необходимые при создании объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0ea21-125">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="0ea21-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="0ea21-126">Parameter</span></span> | <span data-ttu-id="0ea21-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0ea21-127">Type</span></span> | <span data-ttu-id="0ea21-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea21-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ea21-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0ea21-129">displayName</span></span> |<span data-ttu-id="0ea21-130">string</span><span class="sxs-lookup"><span data-stu-id="0ea21-130">string</span></span> |<span data-ttu-id="0ea21-131">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="0ea21-131">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="0ea21-132">состав</span><span class="sxs-lookup"><span data-stu-id="0ea21-132">feature</span></span> |<span data-ttu-id="0ea21-133">стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="0ea21-133">stagedFeatureName</span></span> |<span data-ttu-id="0ea21-134">Компонент, который будет выполнен с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ea21-134">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="0ea21-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0ea21-135">isEnabled</span></span> |<span data-ttu-id="0ea21-136">строка</span><span class="sxs-lookup"><span data-stu-id="0ea21-136">string</span></span> |<span data-ttu-id="0ea21-137">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="0ea21-137">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="0ea21-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea21-138">Response</span></span>

<span data-ttu-id="0ea21-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea21-139">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ea21-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ea21-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ea21-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ea21-141">Request</span></span>

<span data-ttu-id="0ea21-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ea21-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ea21-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea21-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ea21-144">C#</span><span class="sxs-lookup"><span data-stu-id="0ea21-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ea21-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea21-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ea21-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea21-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ea21-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea21-147">Response</span></span>

<span data-ttu-id="0ea21-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea21-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0ea21-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea21-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
