---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ea8cfbab59acde4c6b6e2468d26e6ed9620d9652
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582326"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="18474-104">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="18474-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="18474-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18474-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18474-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="18474-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="18474-107">Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="18474-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="18474-108">Дополнительные сведения см. в [документации по условному доступу](/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="18474-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="18474-109">Методы</span><span class="sxs-lookup"><span data-stu-id="18474-109">Methods</span></span>

| <span data-ttu-id="18474-110">Метод</span><span class="sxs-lookup"><span data-stu-id="18474-110">Method</span></span>       | <span data-ttu-id="18474-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18474-111">Return Type</span></span> | <span data-ttu-id="18474-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18474-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="18474-113">Список КондитионалакцессполиЦиес</span><span class="sxs-lookup"><span data-stu-id="18474-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="18474-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="18474-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="18474-115">Получение всех объектов КондитионалакцессполиЦиес в Организации.</span><span class="sxs-lookup"><span data-stu-id="18474-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="18474-116">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="18474-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="18474-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="18474-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="18474-118">Создание нового объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="18474-119">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="18474-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="18474-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="18474-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="18474-121">Чтение свойств и связей объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="18474-122">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="18474-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="18474-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="18474-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="18474-124">Обновление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="18474-125">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="18474-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="18474-126">Нет</span><span class="sxs-lookup"><span data-stu-id="18474-126">None</span></span> | <span data-ttu-id="18474-127">Удаление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="18474-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="18474-128">Properties</span></span>

| <span data-ttu-id="18474-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18474-129">Property</span></span>     | <span data-ttu-id="18474-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18474-130">Type</span></span>        | <span data-ttu-id="18474-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18474-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18474-132">conditions</span><span class="sxs-lookup"><span data-stu-id="18474-132">conditions</span></span>|[<span data-ttu-id="18474-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="18474-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="18474-134">Задает правила, которые должны выполняться для применения политики.</span><span class="sxs-lookup"><span data-stu-id="18474-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="18474-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18474-135">Required.</span></span> |
|<span data-ttu-id="18474-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18474-136">createdDateTime</span></span>|<span data-ttu-id="18474-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18474-137">DateTimeOffset</span></span>| <span data-ttu-id="18474-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="18474-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18474-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="18474-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="18474-140">Статического.</span><span class="sxs-lookup"><span data-stu-id="18474-140">Readonly.</span></span> |
|<span data-ttu-id="18474-141">displayName</span><span class="sxs-lookup"><span data-stu-id="18474-141">displayName</span></span>|<span data-ttu-id="18474-142">String</span><span class="sxs-lookup"><span data-stu-id="18474-142">String</span></span>| <span data-ttu-id="18474-143">Задает отображаемое имя для объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-143">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="18474-144">грантконтролс</span><span class="sxs-lookup"><span data-stu-id="18474-144">grantControls</span></span>|[<span data-ttu-id="18474-145">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="18474-145">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="18474-146">Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="18474-146">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="18474-147">id</span><span class="sxs-lookup"><span data-stu-id="18474-147">id</span></span>|<span data-ttu-id="18474-148">String</span><span class="sxs-lookup"><span data-stu-id="18474-148">String</span></span>| <span data-ttu-id="18474-149">Задает идентификатор объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-149">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="18474-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18474-150">Read-only.</span></span>|
|<span data-ttu-id="18474-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18474-151">modifiedDateTime</span></span>| <span data-ttu-id="18474-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18474-152">DateTimeOffset</span></span>|<span data-ttu-id="18474-153">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="18474-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18474-154">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="18474-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="18474-155">Статического.</span><span class="sxs-lookup"><span data-stu-id="18474-155">Readonly.</span></span> |
|<span data-ttu-id="18474-156">сессионконтролс</span><span class="sxs-lookup"><span data-stu-id="18474-156">sessionControls</span></span>|[<span data-ttu-id="18474-157">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="18474-157">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="18474-158">Задает элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="18474-158">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="18474-159">состояние</span><span class="sxs-lookup"><span data-stu-id="18474-159">state</span></span>|<span data-ttu-id="18474-160">string</span><span class="sxs-lookup"><span data-stu-id="18474-160">string</span></span>| <span data-ttu-id="18474-161">Задает состояние объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="18474-161">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="18474-162">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="18474-162">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="18474-163">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18474-163">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="18474-164">Связи</span><span class="sxs-lookup"><span data-stu-id="18474-164">Relationships</span></span>

<span data-ttu-id="18474-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="18474-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18474-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="18474-166">JSON representation</span></span>

<span data-ttu-id="18474-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18474-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
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