---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74270d2362bdfd6bbda567c17a45353eda7c319e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031741"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="5d12b-104">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="5d12b-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="5d12b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d12b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d12b-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5d12b-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="5d12b-107">Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="5d12b-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="5d12b-108">Дополнительные сведения см. в [документации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="5d12b-108">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="5d12b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5d12b-109">Methods</span></span>

| <span data-ttu-id="5d12b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5d12b-110">Method</span></span>       | <span data-ttu-id="5d12b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d12b-111">Return Type</span></span> | <span data-ttu-id="5d12b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5d12b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5d12b-113">Список КондитионалакцессполиЦиес</span><span class="sxs-lookup"><span data-stu-id="5d12b-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="5d12b-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d12b-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="5d12b-115">Получение всех объектов КондитионалакцессполиЦиес в Организации.</span><span class="sxs-lookup"><span data-stu-id="5d12b-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="5d12b-116">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="5d12b-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="5d12b-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5d12b-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5d12b-118">Создание нового объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5d12b-119">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="5d12b-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="5d12b-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5d12b-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5d12b-121">Чтение свойств и связей объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5d12b-122">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="5d12b-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="5d12b-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5d12b-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="5d12b-124">Обновление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="5d12b-125">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="5d12b-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="5d12b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="5d12b-126">None</span></span> | <span data-ttu-id="5d12b-127">Удаление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d12b-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d12b-128">Properties</span></span>

| <span data-ttu-id="5d12b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d12b-129">Property</span></span>     | <span data-ttu-id="5d12b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5d12b-130">Type</span></span>        | <span data-ttu-id="5d12b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5d12b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d12b-132">conditions</span><span class="sxs-lookup"><span data-stu-id="5d12b-132">conditions</span></span>|[<span data-ttu-id="5d12b-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="5d12b-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="5d12b-134">Задает правила, которые должны выполняться для применения политики.</span><span class="sxs-lookup"><span data-stu-id="5d12b-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="5d12b-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d12b-135">Required.</span></span> |
|<span data-ttu-id="5d12b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d12b-136">createdDateTime</span></span>|<span data-ttu-id="5d12b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d12b-137">DateTimeOffset</span></span>| <span data-ttu-id="5d12b-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5d12b-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5d12b-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5d12b-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5d12b-140">Статического.</span><span class="sxs-lookup"><span data-stu-id="5d12b-140">Readonly.</span></span> |
|<span data-ttu-id="5d12b-141">description</span><span class="sxs-lookup"><span data-stu-id="5d12b-141">description</span></span>|<span data-ttu-id="5d12b-142">String</span><span class="sxs-lookup"><span data-stu-id="5d12b-142">String</span></span>| <span data-ttu-id="5d12b-143">Не используется.</span><span class="sxs-lookup"><span data-stu-id="5d12b-143">Not used.</span></span> |
|<span data-ttu-id="5d12b-144">displayName</span><span class="sxs-lookup"><span data-stu-id="5d12b-144">displayName</span></span>|<span data-ttu-id="5d12b-145">String</span><span class="sxs-lookup"><span data-stu-id="5d12b-145">String</span></span>| <span data-ttu-id="5d12b-146">Задает отображаемое имя для объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="5d12b-147">грантконтролс</span><span class="sxs-lookup"><span data-stu-id="5d12b-147">grantControls</span></span>|[<span data-ttu-id="5d12b-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="5d12b-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="5d12b-149">Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="5d12b-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="5d12b-150">id</span><span class="sxs-lookup"><span data-stu-id="5d12b-150">id</span></span>|<span data-ttu-id="5d12b-151">String</span><span class="sxs-lookup"><span data-stu-id="5d12b-151">String</span></span>| <span data-ttu-id="5d12b-152">Задает идентификатор объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="5d12b-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d12b-153">Read-only.</span></span>|
|<span data-ttu-id="5d12b-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d12b-154">modifiedDateTime</span></span>| <span data-ttu-id="5d12b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d12b-155">DateTimeOffset</span></span>|<span data-ttu-id="5d12b-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5d12b-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5d12b-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5d12b-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5d12b-158">Статического.</span><span class="sxs-lookup"><span data-stu-id="5d12b-158">Readonly.</span></span> |
|<span data-ttu-id="5d12b-159">сессионконтролс</span><span class="sxs-lookup"><span data-stu-id="5d12b-159">sessionControls</span></span>|[<span data-ttu-id="5d12b-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="5d12b-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="5d12b-161">Задает элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="5d12b-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="5d12b-162">состояние</span><span class="sxs-lookup"><span data-stu-id="5d12b-162">state</span></span>|<span data-ttu-id="5d12b-163">string</span><span class="sxs-lookup"><span data-stu-id="5d12b-163">string</span></span>| <span data-ttu-id="5d12b-164">Задает состояние объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="5d12b-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="5d12b-165">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="5d12b-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="5d12b-166">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="5d12b-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5d12b-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d12b-167">Relationships</span></span>

<span data-ttu-id="5d12b-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5d12b-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d12b-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d12b-169">JSON representation</span></span>

<span data-ttu-id="5d12b-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d12b-170">The following is a JSON representation of the resource.</span></span>

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


