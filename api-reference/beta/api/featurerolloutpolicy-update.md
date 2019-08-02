---
title: Обновление Феатурероллаутполици
description: Обновление свойств объекта феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdbe19a401f10acead10884f02de5d380465e0a
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062171"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="03232-103">Обновление феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="03232-103">Update featurerolloutpolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03232-104">Обновление свойств объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="03232-104">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03232-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03232-105">Permissions</span></span>

<span data-ttu-id="03232-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03232-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03232-108">Permission type</span></span>                        | <span data-ttu-id="03232-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03232-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03232-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03232-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="03232-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="03232-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="03232-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03232-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03232-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03232-113">Not supported.</span></span> |
| <span data-ttu-id="03232-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03232-114">Application</span></span>                            | <span data-ttu-id="03232-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03232-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03232-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03232-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03232-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03232-117">Request headers</span></span>

| <span data-ttu-id="03232-118">Имя</span><span class="sxs-lookup"><span data-stu-id="03232-118">Name</span></span>       | <span data-ttu-id="03232-119">Описание</span><span class="sxs-lookup"><span data-stu-id="03232-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03232-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03232-120">Authorization</span></span> | <span data-ttu-id="03232-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="03232-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="03232-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03232-122">Request body</span></span>

<span data-ttu-id="03232-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="03232-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="03232-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="03232-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="03232-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="03232-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03232-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="03232-126">Property</span></span>     | <span data-ttu-id="03232-127">Тип</span><span class="sxs-lookup"><span data-stu-id="03232-127">Type</span></span>        | <span data-ttu-id="03232-128">Описание</span><span class="sxs-lookup"><span data-stu-id="03232-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03232-129">description</span><span class="sxs-lookup"><span data-stu-id="03232-129">description</span></span>|<span data-ttu-id="03232-130">String</span><span class="sxs-lookup"><span data-stu-id="03232-130">String</span></span>|<span data-ttu-id="03232-131">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="03232-131">A description for this policy.</span></span>|
|<span data-ttu-id="03232-132">displayName</span><span class="sxs-lookup"><span data-stu-id="03232-132">displayName</span></span>|<span data-ttu-id="03232-133">Строка</span><span class="sxs-lookup"><span data-stu-id="03232-133">String</span></span>|<span data-ttu-id="03232-134">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03232-134">The display name for this policy.</span></span>|
|<span data-ttu-id="03232-135">Исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="03232-135">isAppliedToOrganization</span></span>|<span data-ttu-id="03232-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="03232-136">Boolean</span></span>|<span data-ttu-id="03232-137">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="03232-137">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="03232-138">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03232-138">isEnabled</span></span>|<span data-ttu-id="03232-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="03232-139">Boolean</span></span>|<span data-ttu-id="03232-140">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="03232-140">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="03232-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="03232-141">Response</span></span>

<span data-ttu-id="03232-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03232-142">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03232-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="03232-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03232-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="03232-144">Request</span></span>

<span data-ttu-id="03232-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03232-145">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03232-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="03232-146">Response</span></span>

<span data-ttu-id="03232-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03232-147">The following is an example of the response.</span></span>

> <span data-ttu-id="03232-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03232-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
