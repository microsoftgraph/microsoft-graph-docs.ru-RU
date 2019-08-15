---
title: Создание Феатурероллаутполици
description: Создание нового объекта Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e495929ad2a927abc837683e6007daea1f8246ad
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417566"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="03767-103">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="03767-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03767-104">Создание нового объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="03767-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03767-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03767-105">Permissions</span></span>

<span data-ttu-id="03767-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03767-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03767-108">Permission type</span></span>                        | <span data-ttu-id="03767-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03767-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03767-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03767-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="03767-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="03767-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="03767-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03767-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03767-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03767-113">Not supported.</span></span> |
| <span data-ttu-id="03767-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03767-114">Application</span></span>                            | <span data-ttu-id="03767-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03767-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03767-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03767-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="03767-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03767-117">Request headers</span></span>

| <span data-ttu-id="03767-118">Имя</span><span class="sxs-lookup"><span data-stu-id="03767-118">Name</span></span>          | <span data-ttu-id="03767-119">Описание</span><span class="sxs-lookup"><span data-stu-id="03767-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03767-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03767-120">Authorization</span></span> | <span data-ttu-id="03767-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="03767-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="03767-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03767-122">Request body</span></span>

<span data-ttu-id="03767-123">В тексте запроса добавьте представление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03767-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="03767-124">В следующей таблице приведены свойства, необходимые при создании объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="03767-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="03767-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="03767-125">Parameter</span></span> | <span data-ttu-id="03767-126">Тип</span><span class="sxs-lookup"><span data-stu-id="03767-126">Type</span></span> | <span data-ttu-id="03767-127">Описание</span><span class="sxs-lookup"><span data-stu-id="03767-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03767-128">displayName</span><span class="sxs-lookup"><span data-stu-id="03767-128">displayName</span></span> |<span data-ttu-id="03767-129">string</span><span class="sxs-lookup"><span data-stu-id="03767-129">string</span></span> |<span data-ttu-id="03767-130">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="03767-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="03767-131">состав</span><span class="sxs-lookup"><span data-stu-id="03767-131">feature</span></span> |<span data-ttu-id="03767-132">стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="03767-132">stagedFeatureName</span></span> |<span data-ttu-id="03767-133">Компонент, который будет выполнен с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="03767-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="03767-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03767-134">isEnabled</span></span> |<span data-ttu-id="03767-135">string</span><span class="sxs-lookup"><span data-stu-id="03767-135">string</span></span> |<span data-ttu-id="03767-136">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="03767-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="03767-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="03767-137">Response</span></span>

<span data-ttu-id="03767-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03767-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03767-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="03767-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03767-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="03767-140">Request</span></span>

<span data-ttu-id="03767-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03767-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03767-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="03767-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="03767-143">C#</span><span class="sxs-lookup"><span data-stu-id="03767-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03767-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03767-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03767-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="03767-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="03767-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="03767-146">Response</span></span>

<span data-ttu-id="03767-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03767-147">The following is an example of the response.</span></span>

> <span data-ttu-id="03767-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03767-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
