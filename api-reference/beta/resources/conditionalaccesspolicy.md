---
title: тип ресурса conditionalAccessPolicy
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a1ec10d2a64017eac4894d947b5da20802a38c96
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444310"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="0146b-104">тип ресурса conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="0146b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0146b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0146b-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0146b-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="0146b-107">Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.</span><span class="sxs-lookup"><span data-stu-id="0146b-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="0146b-108">Дополнительные сведения см. в [документации условного доступа.](/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="0146b-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="0146b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0146b-109">Methods</span></span>

| <span data-ttu-id="0146b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0146b-110">Method</span></span>       | <span data-ttu-id="0146b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0146b-111">Return Type</span></span> | <span data-ttu-id="0146b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0146b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0146b-113">Список conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="0146b-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="0146b-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0146b-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="0146b-115">Получите все объекты conditionalAccessPolicies в организации.</span><span class="sxs-lookup"><span data-stu-id="0146b-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="0146b-116">Создание conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="0146b-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="0146b-118">Создайте новый объект conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="0146b-119">Get conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="0146b-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="0146b-121">Чтение свойств и связей объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="0146b-122">Обновление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="0146b-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="0146b-124">Обновление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="0146b-125">Удаление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0146b-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="0146b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0146b-126">None</span></span> | <span data-ttu-id="0146b-127">Удаление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0146b-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="0146b-128">Properties</span></span>

| <span data-ttu-id="0146b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0146b-129">Property</span></span>     | <span data-ttu-id="0146b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0146b-130">Type</span></span>        | <span data-ttu-id="0146b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0146b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0146b-132">conditions</span><span class="sxs-lookup"><span data-stu-id="0146b-132">conditions</span></span>|[<span data-ttu-id="0146b-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="0146b-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="0146b-134">Указывает правила, которые необходимо соблюдать для применения политики.</span><span class="sxs-lookup"><span data-stu-id="0146b-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="0146b-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0146b-135">Required.</span></span> |
|<span data-ttu-id="0146b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0146b-136">createdDateTime</span></span>|<span data-ttu-id="0146b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0146b-137">DateTimeOffset</span></span>| <span data-ttu-id="0146b-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0146b-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0146b-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0146b-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0146b-140">Readonly.</span><span class="sxs-lookup"><span data-stu-id="0146b-140">Readonly.</span></span> |
|<span data-ttu-id="0146b-141">description</span><span class="sxs-lookup"><span data-stu-id="0146b-141">description</span></span>|<span data-ttu-id="0146b-142">String</span><span class="sxs-lookup"><span data-stu-id="0146b-142">String</span></span>| <span data-ttu-id="0146b-143">Не используется.</span><span class="sxs-lookup"><span data-stu-id="0146b-143">Not used.</span></span> |
|<span data-ttu-id="0146b-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0146b-144">displayName</span></span>|<span data-ttu-id="0146b-145">String</span><span class="sxs-lookup"><span data-stu-id="0146b-145">String</span></span>| <span data-ttu-id="0146b-146">Указывает имя отображения объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="0146b-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="0146b-147">grantControls</span></span>|[<span data-ttu-id="0146b-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="0146b-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="0146b-149">Указывает элементы управления грантами, которые необходимо выполнить для выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="0146b-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="0146b-150">id</span><span class="sxs-lookup"><span data-stu-id="0146b-150">id</span></span>|<span data-ttu-id="0146b-151">String</span><span class="sxs-lookup"><span data-stu-id="0146b-151">String</span></span>| <span data-ttu-id="0146b-152">Указывает идентификатор объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="0146b-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0146b-153">Read-only.</span></span>|
|<span data-ttu-id="0146b-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0146b-154">modifiedDateTime</span></span>| <span data-ttu-id="0146b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0146b-155">DateTimeOffset</span></span>|<span data-ttu-id="0146b-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0146b-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0146b-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0146b-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0146b-158">Readonly.</span><span class="sxs-lookup"><span data-stu-id="0146b-158">Readonly.</span></span> |
|<span data-ttu-id="0146b-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="0146b-159">sessionControls</span></span>|[<span data-ttu-id="0146b-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="0146b-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="0146b-161">Указывает элементы управления сеансами, которые применяются после регистрации.</span><span class="sxs-lookup"><span data-stu-id="0146b-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="0146b-162">состояние</span><span class="sxs-lookup"><span data-stu-id="0146b-162">state</span></span>|<span data-ttu-id="0146b-163">string</span><span class="sxs-lookup"><span data-stu-id="0146b-163">string</span></span>| <span data-ttu-id="0146b-164">Указывает состояние объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0146b-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="0146b-165">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="0146b-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="0146b-166">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0146b-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0146b-167">Связи</span><span class="sxs-lookup"><span data-stu-id="0146b-167">Relationships</span></span>

<span data-ttu-id="0146b-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0146b-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0146b-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0146b-169">JSON representation</span></span>

<span data-ttu-id="0146b-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0146b-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "keyProperty": "id"
}-->

```json
{
  "conditions": {"@odata.type": "microsoft.graph.conditionalAccessConditionSet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "grantControls": {"@odata.type": "microsoft.graph.conditionalAccessGrantControls"},
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)",
  "sessionControls": {"@odata.type": "microsoft.graph.conditionalAccessSessionControls"},
  "state": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
