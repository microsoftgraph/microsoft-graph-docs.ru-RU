---
title: тип ресурса conditionalAccessPolicy
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 578d7cfcab984922d0c98f7cc8971daf9b10a2fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958817"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="d1947-104">тип ресурса conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="d1947-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1947-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1947-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1947-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="d1947-107">Политики условного доступа — это настраиваемые правила, определяемые сценарием доступа.</span><span class="sxs-lookup"><span data-stu-id="d1947-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="d1947-108">Дополнительные сведения см. в [документации условного доступа.](/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="d1947-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="d1947-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d1947-109">Methods</span></span>

| <span data-ttu-id="d1947-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d1947-110">Method</span></span>       | <span data-ttu-id="d1947-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d1947-111">Return Type</span></span> | <span data-ttu-id="d1947-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d1947-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d1947-113">Список conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="d1947-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="d1947-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d1947-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="d1947-115">Получите все объекты conditionalAccessPolicies в организации.</span><span class="sxs-lookup"><span data-stu-id="d1947-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="d1947-116">Создание conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="d1947-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="d1947-118">Создайте новый объект conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="d1947-119">Get conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="d1947-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="d1947-121">Чтение свойств и связей объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="d1947-122">Обновление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="d1947-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="d1947-124">Обновление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="d1947-125">Удаление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d1947-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="d1947-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d1947-126">None</span></span> | <span data-ttu-id="d1947-127">Удаление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d1947-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1947-128">Properties</span></span>

| <span data-ttu-id="d1947-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1947-129">Property</span></span>     | <span data-ttu-id="d1947-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d1947-130">Type</span></span>        | <span data-ttu-id="d1947-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d1947-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d1947-132">conditions</span><span class="sxs-lookup"><span data-stu-id="d1947-132">conditions</span></span>|[<span data-ttu-id="d1947-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="d1947-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="d1947-134">Указывает правила, которые необходимо соблюдать для применения политики.</span><span class="sxs-lookup"><span data-stu-id="d1947-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="d1947-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1947-135">Required.</span></span> |
|<span data-ttu-id="d1947-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1947-136">createdDateTime</span></span>|<span data-ttu-id="d1947-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1947-137">DateTimeOffset</span></span>| <span data-ttu-id="d1947-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d1947-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d1947-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d1947-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d1947-140">Readonly.</span><span class="sxs-lookup"><span data-stu-id="d1947-140">Readonly.</span></span> |
|<span data-ttu-id="d1947-141">description</span><span class="sxs-lookup"><span data-stu-id="d1947-141">description</span></span>|<span data-ttu-id="d1947-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d1947-142">String</span></span>| <span data-ttu-id="d1947-143">Не используется.</span><span class="sxs-lookup"><span data-stu-id="d1947-143">Not used.</span></span> |
|<span data-ttu-id="d1947-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d1947-144">displayName</span></span>|<span data-ttu-id="d1947-145">Строка</span><span class="sxs-lookup"><span data-stu-id="d1947-145">String</span></span>| <span data-ttu-id="d1947-146">Указывает имя отображения объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="d1947-147">grantControls</span><span class="sxs-lookup"><span data-stu-id="d1947-147">grantControls</span></span>|[<span data-ttu-id="d1947-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="d1947-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="d1947-149">Указывает элементы управления грантами, которые необходимо выполнить для выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="d1947-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="d1947-150">id</span><span class="sxs-lookup"><span data-stu-id="d1947-150">id</span></span>|<span data-ttu-id="d1947-151">Строка</span><span class="sxs-lookup"><span data-stu-id="d1947-151">String</span></span>| <span data-ttu-id="d1947-152">Указывает идентификатор объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="d1947-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1947-153">Read-only.</span></span>|
|<span data-ttu-id="d1947-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1947-154">modifiedDateTime</span></span>| <span data-ttu-id="d1947-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1947-155">DateTimeOffset</span></span>|<span data-ttu-id="d1947-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d1947-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d1947-157">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d1947-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d1947-158">Readonly.</span><span class="sxs-lookup"><span data-stu-id="d1947-158">Readonly.</span></span> |
|<span data-ttu-id="d1947-159">sessionControls</span><span class="sxs-lookup"><span data-stu-id="d1947-159">sessionControls</span></span>|[<span data-ttu-id="d1947-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="d1947-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="d1947-161">Указывает элементы управления сеансами, которые применяются после регистрации.</span><span class="sxs-lookup"><span data-stu-id="d1947-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="d1947-162">state</span><span class="sxs-lookup"><span data-stu-id="d1947-162">state</span></span>|<span data-ttu-id="d1947-163">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="d1947-163">conditionalAccessPolicyState</span></span>| <span data-ttu-id="d1947-164">Указывает состояние объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="d1947-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="d1947-165">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="d1947-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="d1947-166">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1947-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d1947-167">Связи</span><span class="sxs-lookup"><span data-stu-id="d1947-167">Relationships</span></span>

<span data-ttu-id="d1947-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1947-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1947-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d1947-169">JSON representation</span></span>

<span data-ttu-id="d1947-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1947-170">The following is a JSON representation of the resource.</span></span>

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
