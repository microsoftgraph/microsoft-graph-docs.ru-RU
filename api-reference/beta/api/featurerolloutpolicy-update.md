---
title: Обновление функцииRolloutPolicy
description: Обновление свойств объекта featurerolloutpolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 26d5f16bd6d61689ff4cfe73b83c4a45add9c2f7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471105"
---
# <a name="update-featurerolloutpolicy"></a><span data-ttu-id="30ea6-103">Обновление featurerolloutpolicy</span><span class="sxs-lookup"><span data-stu-id="30ea6-103">Update featurerolloutpolicy</span></span>

<span data-ttu-id="30ea6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30ea6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30ea6-105">Обновление свойств [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="30ea6-105">Update the properties of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30ea6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30ea6-106">Permissions</span></span>

<span data-ttu-id="30ea6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30ea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30ea6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30ea6-109">Permission type</span></span>                        | <span data-ttu-id="30ea6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30ea6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="30ea6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30ea6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="30ea6-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30ea6-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="30ea6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30ea6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30ea6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30ea6-114">Not supported.</span></span> |
| <span data-ttu-id="30ea6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30ea6-115">Application</span></span>                            | <span data-ttu-id="30ea6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30ea6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30ea6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30ea6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="30ea6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30ea6-118">Request headers</span></span>

| <span data-ttu-id="30ea6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="30ea6-119">Name</span></span>       | <span data-ttu-id="30ea6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="30ea6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="30ea6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30ea6-121">Authorization</span></span> | <span data-ttu-id="30ea6-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="30ea6-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="30ea6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30ea6-123">Request body</span></span>

<span data-ttu-id="30ea6-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="30ea6-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="30ea6-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="30ea6-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="30ea6-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="30ea6-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="30ea6-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="30ea6-127">Property</span></span>     | <span data-ttu-id="30ea6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="30ea6-128">Type</span></span>        | <span data-ttu-id="30ea6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="30ea6-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="30ea6-130">description</span><span class="sxs-lookup"><span data-stu-id="30ea6-130">description</span></span>|<span data-ttu-id="30ea6-131">String</span><span class="sxs-lookup"><span data-stu-id="30ea6-131">String</span></span>|<span data-ttu-id="30ea6-132">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="30ea6-132">A description for this policy.</span></span>|
|<span data-ttu-id="30ea6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="30ea6-133">displayName</span></span>|<span data-ttu-id="30ea6-134">String</span><span class="sxs-lookup"><span data-stu-id="30ea6-134">String</span></span>|<span data-ttu-id="30ea6-135">Имя отображения для этой политики.</span><span class="sxs-lookup"><span data-stu-id="30ea6-135">The display name for this policy.</span></span>|
|<span data-ttu-id="30ea6-136">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="30ea6-136">isAppliedToOrganization</span></span>|<span data-ttu-id="30ea6-137">Логический</span><span class="sxs-lookup"><span data-stu-id="30ea6-137">Boolean</span></span>|<span data-ttu-id="30ea6-138">Указывает, следует ли применять эту политику выкатки функций ко всей организации.</span><span class="sxs-lookup"><span data-stu-id="30ea6-138">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="30ea6-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="30ea6-139">isEnabled</span></span>|<span data-ttu-id="30ea6-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="30ea6-140">Boolean</span></span>|<span data-ttu-id="30ea6-141">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="30ea6-141">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="response"></a><span data-ttu-id="30ea6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="30ea6-142">Response</span></span>

<span data-ttu-id="30ea6-143">В случае успешной работы этот метод возвращает код ответа и `200 OK` обновленный [объект featureRolloutPolicy](../resources/featurerolloutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="30ea6-143">If successful, this method returns a `200 OK` response code and an updated [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30ea6-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="30ea6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30ea6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="30ea6-145">Request</span></span>

<span data-ttu-id="30ea6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30ea6-146">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30ea6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="30ea6-147">Response</span></span>

<span data-ttu-id="30ea6-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30ea6-148">The following is an example of the response.</span></span>

> <span data-ttu-id="30ea6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30ea6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


