---
title: Тип ресурса conditionalAccessPolicy
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, которые определяют сценарий доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55517d33e7ae933e360118b36b56ad8e8088b50a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153468"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="5c609-104">Тип ресурса conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="5c609-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c609-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c609-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5c609-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="5c609-107">Политики условного доступа — это настраиваемые правила, которые определяют сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="5c609-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="5c609-108">Дополнительные сведения см. в [документации по условному доступу.](/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="5c609-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="5c609-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5c609-109">Methods</span></span>

| <span data-ttu-id="5c609-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5c609-110">Method</span></span>       | <span data-ttu-id="5c609-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c609-111">Return Type</span></span> | <span data-ttu-id="5c609-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5c609-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5c609-113">Список conditionalAccessPolicies</span><span class="sxs-lookup"><span data-stu-id="5c609-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="5c609-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5c609-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="5c609-115">Получите все объекты conditionalAccessPolicies в организации.</span><span class="sxs-lookup"><span data-stu-id="5c609-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="5c609-116">Создание conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="5c609-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5c609-118">Создание объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5c609-119">Get conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="5c609-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5c609-121">Чтение свойств и связей объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5c609-122">Обновление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="5c609-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5c609-124">Обновление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5c609-125">Удаление conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5c609-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="5c609-126">Нет</span><span class="sxs-lookup"><span data-stu-id="5c609-126">None</span></span> | <span data-ttu-id="5c609-127">Удаление объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c609-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c609-128">Properties</span></span>

| <span data-ttu-id="5c609-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c609-129">Property</span></span>     | <span data-ttu-id="5c609-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c609-130">Type</span></span>        | <span data-ttu-id="5c609-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c609-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c609-132">conditions</span><span class="sxs-lookup"><span data-stu-id="5c609-132">conditions</span></span>|[<span data-ttu-id="5c609-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="5c609-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="5c609-134">Определяет правила, которые должны быть выполнены, чтобы применить политику.</span><span class="sxs-lookup"><span data-stu-id="5c609-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="5c609-135">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="5c609-135">Required.</span></span> |
|<span data-ttu-id="5c609-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c609-136">createdDateTime</span></span>|<span data-ttu-id="5c609-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c609-137">DateTimeOffset</span></span>| <span data-ttu-id="5c609-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5c609-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c609-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5c609-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5c609-140">Readonly.</span><span class="sxs-lookup"><span data-stu-id="5c609-140">Readonly.</span></span> |
|<span data-ttu-id="5c609-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5c609-141">displayName</span></span>|<span data-ttu-id="5c609-142">String</span><span class="sxs-lookup"><span data-stu-id="5c609-142">String</span></span>| <span data-ttu-id="5c609-143">Указывает отображаемое имя объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-143">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="5c609-144">grantControls</span><span class="sxs-lookup"><span data-stu-id="5c609-144">grantControls</span></span>|[<span data-ttu-id="5c609-145">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="5c609-145">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="5c609-146">Указывает элементы управления предоставлением, которые должны быть выполнены для прохода политики.</span><span class="sxs-lookup"><span data-stu-id="5c609-146">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="5c609-147">id</span><span class="sxs-lookup"><span data-stu-id="5c609-147">id</span></span>|<span data-ttu-id="5c609-148">String</span><span class="sxs-lookup"><span data-stu-id="5c609-148">String</span></span>| <span data-ttu-id="5c609-149">Указывает идентификатор объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-149">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="5c609-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c609-150">Read-only.</span></span>|
|<span data-ttu-id="5c609-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c609-151">modifiedDateTime</span></span>| <span data-ttu-id="5c609-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c609-152">DateTimeOffset</span></span>|<span data-ttu-id="5c609-153">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5c609-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c609-154">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5c609-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5c609-155">Readonly.</span><span class="sxs-lookup"><span data-stu-id="5c609-155">Readonly.</span></span> |
|<span data-ttu-id="5c609-156">sessionControls</span><span class="sxs-lookup"><span data-stu-id="5c609-156">sessionControls</span></span>|[<span data-ttu-id="5c609-157">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="5c609-157">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="5c609-158">Указывает элементы управления сеансом, которые применяются после регистрации.</span><span class="sxs-lookup"><span data-stu-id="5c609-158">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="5c609-159">состояние</span><span class="sxs-lookup"><span data-stu-id="5c609-159">state</span></span>|<span data-ttu-id="5c609-160">string</span><span class="sxs-lookup"><span data-stu-id="5c609-160">string</span></span>| <span data-ttu-id="5c609-161">Указывает состояние объекта conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="5c609-161">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="5c609-162">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="5c609-162">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="5c609-163">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c609-163">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5c609-164">Связи</span><span class="sxs-lookup"><span data-stu-id="5c609-164">Relationships</span></span>

<span data-ttu-id="5c609-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5c609-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c609-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5c609-166">JSON representation</span></span>

<span data-ttu-id="5c609-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c609-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
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