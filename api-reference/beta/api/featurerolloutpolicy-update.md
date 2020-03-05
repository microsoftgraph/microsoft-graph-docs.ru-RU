---
title: Обновление Феатурероллаутполици
description: Обновление свойств объекта феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e93dbcbdc7d4a4d40b929a801dae4b673100a274
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421713"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="da897-103">Обновление феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="da897-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="da897-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da897-105">Обновление свойств объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="da897-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da897-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da897-106">Permissions</span></span>

<span data-ttu-id="da897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da897-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da897-109">Permission type</span></span>                        | <span data-ttu-id="da897-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da897-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da897-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da897-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da897-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="da897-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="da897-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da897-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da897-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da897-114">Not supported.</span></span> |
| <span data-ttu-id="da897-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da897-115">Application</span></span>                            | <span data-ttu-id="da897-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da897-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da897-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da897-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da897-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da897-118">Request headers</span></span>

| <span data-ttu-id="da897-119">Имя</span><span class="sxs-lookup"><span data-stu-id="da897-119">Name</span></span>       | <span data-ttu-id="da897-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da897-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da897-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da897-121">Authorization</span></span> | <span data-ttu-id="da897-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="da897-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="da897-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da897-123">Request body</span></span>

<span data-ttu-id="da897-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="da897-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="da897-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="da897-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="da897-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da897-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da897-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="da897-127">Property</span></span>     | <span data-ttu-id="da897-128">Тип</span><span class="sxs-lookup"><span data-stu-id="da897-128">Type</span></span>        | <span data-ttu-id="da897-129">Описание</span><span class="sxs-lookup"><span data-stu-id="da897-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da897-130">description</span><span class="sxs-lookup"><span data-stu-id="da897-130">description</span></span>|<span data-ttu-id="da897-131">String</span><span class="sxs-lookup"><span data-stu-id="da897-131">String</span></span>|<span data-ttu-id="da897-132">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="da897-132">A description for this policy.</span></span>|
|<span data-ttu-id="da897-133">displayName</span><span class="sxs-lookup"><span data-stu-id="da897-133">displayName</span></span>|<span data-ttu-id="da897-134">Строка</span><span class="sxs-lookup"><span data-stu-id="da897-134">String</span></span>|<span data-ttu-id="da897-135">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="da897-135">The display name for this policy.</span></span>|
|<span data-ttu-id="da897-136">исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="da897-136">isAppliedToOrganization</span></span>|<span data-ttu-id="da897-137">Логический</span><span class="sxs-lookup"><span data-stu-id="da897-137">Boolean</span></span>|<span data-ttu-id="da897-138">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="da897-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="da897-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="da897-139">isEnabled</span></span>|<span data-ttu-id="da897-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="da897-140">Boolean</span></span>|<span data-ttu-id="da897-141">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="da897-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="da897-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="da897-142">Response</span></span>

<span data-ttu-id="da897-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da897-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da897-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="da897-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da897-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="da897-145">Request</span></span>

<span data-ttu-id="da897-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da897-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_featurerolloutpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a

Content-type: application/json

{
  "displayName": "PasswordHashSync Rollout Policy",
  "description": "PasswordHashSync Rollout Policy",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a><span data-ttu-id="da897-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="da897-147">Response</span></span>

<span data-ttu-id="da897-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da897-148">The following is an example of the response.</span></span>

> <span data-ttu-id="da897-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da897-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
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
