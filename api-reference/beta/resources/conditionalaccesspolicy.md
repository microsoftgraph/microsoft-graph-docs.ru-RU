---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8291bcd418af5549a8abb7dd30deebcdde9ed03
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636808"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="c1779-104">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c1779-104">conditionalAccessPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1779-105">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1779-105">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="c1779-106">Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="c1779-106">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="c1779-107">Дополнительные сведения см. в [документации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="c1779-107">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="c1779-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c1779-108">Methods</span></span>

| <span data-ttu-id="c1779-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c1779-109">Method</span></span>       | <span data-ttu-id="c1779-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c1779-110">Return Type</span></span> | <span data-ttu-id="c1779-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1779-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c1779-112">Список КондитионалакцессполиЦиес</span><span class="sxs-lookup"><span data-stu-id="c1779-112">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="c1779-113">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c1779-113">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="c1779-114">Получение всех объектов КондитионалакцессполиЦиес в Организации.</span><span class="sxs-lookup"><span data-stu-id="c1779-114">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="c1779-115">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c1779-115">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="c1779-116">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c1779-116">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c1779-117">Создание нового объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-117">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c1779-118">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c1779-118">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="c1779-119">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c1779-119">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c1779-120">Чтение свойств и связей объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-120">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c1779-121">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c1779-121">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="c1779-122">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c1779-122">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c1779-123">Обновление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-123">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c1779-124">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c1779-124">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="c1779-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c1779-125">None</span></span> | <span data-ttu-id="c1779-126">Удаление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-126">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1779-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1779-127">Properties</span></span>

| <span data-ttu-id="c1779-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1779-128">Property</span></span>     | <span data-ttu-id="c1779-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c1779-129">Type</span></span>        | <span data-ttu-id="c1779-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c1779-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1779-131">conditions</span><span class="sxs-lookup"><span data-stu-id="c1779-131">conditions</span></span>|[<span data-ttu-id="c1779-132">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="c1779-132">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="c1779-133">Задает правила, которые должны выполняться для применения политики.</span><span class="sxs-lookup"><span data-stu-id="c1779-133">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="c1779-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1779-134">Required.</span></span> |
|<span data-ttu-id="c1779-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1779-135">createdDateTime</span></span>|<span data-ttu-id="c1779-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1779-136">DateTimeOffset</span></span>| <span data-ttu-id="c1779-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1779-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1779-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c1779-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c1779-139">Статического.</span><span class="sxs-lookup"><span data-stu-id="c1779-139">Readonly.</span></span> |
|<span data-ttu-id="c1779-140">description</span><span class="sxs-lookup"><span data-stu-id="c1779-140">description</span></span>|<span data-ttu-id="c1779-141">String</span><span class="sxs-lookup"><span data-stu-id="c1779-141">String</span></span>| <span data-ttu-id="c1779-142">Не используется.</span><span class="sxs-lookup"><span data-stu-id="c1779-142">Not used.</span></span> |
|<span data-ttu-id="c1779-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c1779-143">displayName</span></span>|<span data-ttu-id="c1779-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c1779-144">String</span></span>| <span data-ttu-id="c1779-145">Задает отображаемое имя для объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-145">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="c1779-146">грантконтролс</span><span class="sxs-lookup"><span data-stu-id="c1779-146">grantControls</span></span>|[<span data-ttu-id="c1779-147">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="c1779-147">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="c1779-148">Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="c1779-148">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="c1779-149">id</span><span class="sxs-lookup"><span data-stu-id="c1779-149">id</span></span>|<span data-ttu-id="c1779-150">String</span><span class="sxs-lookup"><span data-stu-id="c1779-150">String</span></span>| <span data-ttu-id="c1779-151">Задает идентификатор объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-151">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="c1779-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1779-152">Read-only.</span></span>|
|<span data-ttu-id="c1779-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1779-153">modifiedDateTime</span></span>| <span data-ttu-id="c1779-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1779-154">DateTimeOffset</span></span>|<span data-ttu-id="c1779-155">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1779-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1779-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c1779-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c1779-157">Статического.</span><span class="sxs-lookup"><span data-stu-id="c1779-157">Readonly.</span></span> |
|<span data-ttu-id="c1779-158">сессионконтролс</span><span class="sxs-lookup"><span data-stu-id="c1779-158">sessionControls</span></span>|[<span data-ttu-id="c1779-159">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="c1779-159">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="c1779-160">Задает элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="c1779-160">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="c1779-161">состояние</span><span class="sxs-lookup"><span data-stu-id="c1779-161">state</span></span>|<span data-ttu-id="c1779-162">string</span><span class="sxs-lookup"><span data-stu-id="c1779-162">string</span></span>| <span data-ttu-id="c1779-163">Задает состояние объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c1779-163">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="c1779-164">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="c1779-164">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="c1779-165">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="c1779-165">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c1779-166">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1779-166">Relationships</span></span>

<span data-ttu-id="c1779-167">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c1779-167">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1779-168">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1779-168">JSON representation</span></span>

<span data-ttu-id="c1779-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1779-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "baseType": "",
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
