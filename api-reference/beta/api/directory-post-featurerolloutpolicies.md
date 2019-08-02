---
title: Создание Феатурероллаутполици
description: Создание нового объекта Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 716fa19e8fcccc69a33e53a22360638545ec81f5
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062169"
---
# <a name="create-featurerolloutpolicy"></a><span data-ttu-id="00f7c-103">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="00f7c-103">Create featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f7c-104">Создание нового объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="00f7c-104">Create a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00f7c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00f7c-105">Permissions</span></span>

<span data-ttu-id="00f7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00f7c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f7c-108">Permission type</span></span>                        | <span data-ttu-id="00f7c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f7c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="00f7c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f7c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="00f7c-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="00f7c-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="00f7c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f7c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f7c-113">Not supported.</span></span> |
| <span data-ttu-id="00f7c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00f7c-114">Application</span></span>                            | <span data-ttu-id="00f7c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f7c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f7c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f7c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="00f7c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f7c-117">Request headers</span></span>

| <span data-ttu-id="00f7c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="00f7c-118">Name</span></span>          | <span data-ttu-id="00f7c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="00f7c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="00f7c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f7c-120">Authorization</span></span> | <span data-ttu-id="00f7c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="00f7c-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="00f7c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00f7c-122">Request body</span></span>

<span data-ttu-id="00f7c-123">В тексте запроса добавьте представление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00f7c-123">In the request body, supply a JSON representation of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

<span data-ttu-id="00f7c-124">В следующей таблице приведены свойства, необходимые при создании объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="00f7c-124">The following table shows the properties that are required when you create a [featureRolloutPolicy](../resources/featurerolloutpolicy.md).</span></span>

| <span data-ttu-id="00f7c-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="00f7c-125">Parameter</span></span> | <span data-ttu-id="00f7c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="00f7c-126">Type</span></span> | <span data-ttu-id="00f7c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="00f7c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00f7c-128">displayName</span><span class="sxs-lookup"><span data-stu-id="00f7c-128">displayName</span></span> |<span data-ttu-id="00f7c-129">string</span><span class="sxs-lookup"><span data-stu-id="00f7c-129">string</span></span> |<span data-ttu-id="00f7c-130">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="00f7c-130">The display name for this feature rollout policy.</span></span>|
|<span data-ttu-id="00f7c-131">состав</span><span class="sxs-lookup"><span data-stu-id="00f7c-131">feature</span></span> |<span data-ttu-id="00f7c-132">Стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="00f7c-132">stagedFeatureName</span></span> |<span data-ttu-id="00f7c-133">Компонент, который будет выполнен с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="00f7c-133">The feature that would be rolled out using this policy.</span></span>|
|<span data-ttu-id="00f7c-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="00f7c-134">isEnabled</span></span> |<span data-ttu-id="00f7c-135">string</span><span class="sxs-lookup"><span data-stu-id="00f7c-135">string</span></span> |<span data-ttu-id="00f7c-136">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="00f7c-136">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="00f7c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f7c-137">Response</span></span>

<span data-ttu-id="00f7c-138">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00f7c-138">If successful, this method returns a `201 Created` response code and a new [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00f7c-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="00f7c-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00f7c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f7c-140">Request</span></span>

<span data-ttu-id="00f7c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f7c-141">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="00f7c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f7c-142">Response</span></span>

<span data-ttu-id="00f7c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00f7c-143">The following is an example of the response.</span></span>

> <span data-ttu-id="00f7c-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00f7c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
