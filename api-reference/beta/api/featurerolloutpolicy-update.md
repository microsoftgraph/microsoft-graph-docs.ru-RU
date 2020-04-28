---
title: Обновление Феатурероллаутполици
description: Обновление свойств объекта феатурероллаутполици.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1e454f08649b631a694194a585a623e9c819702
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181100"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="86e06-103">Обновление феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="86e06-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="86e06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86e06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86e06-105">Обновление свойств объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="86e06-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86e06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86e06-106">Permissions</span></span>

<span data-ttu-id="86e06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86e06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86e06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86e06-109">Permission type</span></span>                        | <span data-ttu-id="86e06-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86e06-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86e06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86e06-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86e06-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="86e06-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="86e06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86e06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86e06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e06-114">Not supported.</span></span> |
| <span data-ttu-id="86e06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86e06-115">Application</span></span>                            | <span data-ttu-id="86e06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e06-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86e06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86e06-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="86e06-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86e06-118">Request headers</span></span>

| <span data-ttu-id="86e06-119">Имя</span><span class="sxs-lookup"><span data-stu-id="86e06-119">Name</span></span>       | <span data-ttu-id="86e06-120">Описание</span><span class="sxs-lookup"><span data-stu-id="86e06-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86e06-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86e06-121">Authorization</span></span> | <span data-ttu-id="86e06-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="86e06-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86e06-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86e06-123">Request body</span></span>

<span data-ttu-id="86e06-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="86e06-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="86e06-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="86e06-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="86e06-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="86e06-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86e06-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="86e06-127">Property</span></span>     | <span data-ttu-id="86e06-128">Тип</span><span class="sxs-lookup"><span data-stu-id="86e06-128">Type</span></span>        | <span data-ttu-id="86e06-129">Описание</span><span class="sxs-lookup"><span data-stu-id="86e06-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86e06-130">description</span><span class="sxs-lookup"><span data-stu-id="86e06-130">description</span></span>|<span data-ttu-id="86e06-131">String</span><span class="sxs-lookup"><span data-stu-id="86e06-131">String</span></span>|<span data-ttu-id="86e06-132">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="86e06-132">A description for this policy.</span></span>|
|<span data-ttu-id="86e06-133">displayName</span><span class="sxs-lookup"><span data-stu-id="86e06-133">displayName</span></span>|<span data-ttu-id="86e06-134">Строка</span><span class="sxs-lookup"><span data-stu-id="86e06-134">String</span></span>|<span data-ttu-id="86e06-135">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86e06-135">The display name for this policy.</span></span>|
|<span data-ttu-id="86e06-136">исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="86e06-136">isAppliedToOrganization</span></span>|<span data-ttu-id="86e06-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="86e06-137">Boolean</span></span>|<span data-ttu-id="86e06-138">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="86e06-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="86e06-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="86e06-139">isEnabled</span></span>|<span data-ttu-id="86e06-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="86e06-140">Boolean</span></span>|<span data-ttu-id="86e06-141">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="86e06-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="86e06-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="86e06-142">Response</span></span>

<span data-ttu-id="86e06-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86e06-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86e06-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="86e06-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86e06-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="86e06-145">Request</span></span>

<span data-ttu-id="86e06-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86e06-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86e06-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="86e06-147">Response</span></span>

<span data-ttu-id="86e06-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86e06-148">The following is an example of the response.</span></span>

> <span data-ttu-id="86e06-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86e06-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
