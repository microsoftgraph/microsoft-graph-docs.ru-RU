---
title: Создание Феатурероллаутполици
description: Создание нового объекта Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ebdf62079324be390868274fa9bd1c7e22ac4e1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172973"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="10374-103">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="10374-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10374-104">Создание нового объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="10374-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10374-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10374-105">Permissions</span></span>

<span data-ttu-id="10374-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10374-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10374-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10374-108">Permission type</span></span>                        | <span data-ttu-id="10374-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10374-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10374-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10374-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="10374-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="10374-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="10374-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10374-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10374-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10374-113">Not supported.</span></span> |
| <span data-ttu-id="10374-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10374-114">Application</span></span>                            | <span data-ttu-id="10374-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10374-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10374-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10374-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="10374-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10374-117">Request headers</span></span>

| <span data-ttu-id="10374-118">Имя</span><span class="sxs-lookup"><span data-stu-id="10374-118">Name</span></span>          | <span data-ttu-id="10374-119">Описание</span><span class="sxs-lookup"><span data-stu-id="10374-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10374-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10374-120">Authorization</span></span> | <span data-ttu-id="10374-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="10374-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10374-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10374-122">Request body</span></span>

<span data-ttu-id="10374-123">В тексте запроса добавьте представление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10374-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="10374-124">В следующей таблице приведены свойства, необходимые при создании объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10374-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="10374-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="10374-125">Parameter</span></span> | <span data-ttu-id="10374-126">Тип</span><span class="sxs-lookup"><span data-stu-id="10374-126">Type</span></span> | <span data-ttu-id="10374-127">Описание</span><span class="sxs-lookup"><span data-stu-id="10374-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10374-128">displayName</span><span class="sxs-lookup"><span data-stu-id="10374-128">displayName</span></span> |<span data-ttu-id="10374-129">string</span><span class="sxs-lookup"><span data-stu-id="10374-129">string</span></span> |<span data-ttu-id="10374-130">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="10374-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="10374-131">состав</span><span class="sxs-lookup"><span data-stu-id="10374-131">feature</span></span> |<span data-ttu-id="10374-132">Стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="10374-132">stagedFeatureName</span></span> |<span data-ttu-id="10374-133">Компонент, который будет выполнен с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="10374-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="10374-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="10374-134">isEnabled</span></span> |<span data-ttu-id="10374-135">string</span><span class="sxs-lookup"><span data-stu-id="10374-135">string</span></span> |<span data-ttu-id="10374-136">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="10374-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="10374-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10374-137">Response</span></span>

<span data-ttu-id="10374-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10374-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10374-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="10374-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10374-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="10374-140">Request</span></span>

<span data-ttu-id="10374-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10374-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="10374-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="10374-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="10374-143">C#</span><span class="sxs-lookup"><span data-stu-id="10374-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-featurerolloutpolicy-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10374-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="10374-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-featurerolloutpolicy-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10374-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="10374-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-featurerolloutpolicy-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="10374-146">Java</span><span class="sxs-lookup"><span data-stu-id="10374-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-featurerolloutpolicy-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10374-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="10374-147">Response</span></span>

<span data-ttu-id="10374-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10374-148">The following is an example of the response.</span></span>

> <span data-ttu-id="10374-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10374-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
