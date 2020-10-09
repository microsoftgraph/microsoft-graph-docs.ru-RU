---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 70ba87f751c7dc61a71578b845df9978b7148f60
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402984"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="c5e1c-104">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c5e1c-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="c5e1c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5e1c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5e1c-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="c5e1c-107">Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="c5e1c-108">Дополнительные сведения см. в [документации по условному доступу](/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="c5e1c-108">For more information, see the [Conditional access documentation](/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="c5e1c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c5e1c-109">Methods</span></span>

| <span data-ttu-id="c5e1c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c5e1c-110">Method</span></span>       | <span data-ttu-id="c5e1c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c5e1c-111">Return Type</span></span> | <span data-ttu-id="c5e1c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e1c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c5e1c-113">Список КондитионалакцессполиЦиес</span><span class="sxs-lookup"><span data-stu-id="c5e1c-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="c5e1c-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c5e1c-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="c5e1c-115">Получение всех объектов КондитионалакцессполиЦиес в Организации.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="c5e1c-116">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c5e1c-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="c5e1c-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c5e1c-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c5e1c-118">Создание нового объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c5e1c-119">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c5e1c-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="c5e1c-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c5e1c-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c5e1c-121">Чтение свойств и связей объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c5e1c-122">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c5e1c-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="c5e1c-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="c5e1c-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="c5e1c-124">Обновление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="c5e1c-125">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="c5e1c-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="c5e1c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c5e1c-126">None</span></span> | <span data-ttu-id="c5e1c-127">Удаление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5e1c-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5e1c-128">Properties</span></span>

| <span data-ttu-id="c5e1c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5e1c-129">Property</span></span>     | <span data-ttu-id="c5e1c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c5e1c-130">Type</span></span>        | <span data-ttu-id="c5e1c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e1c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5e1c-132">conditions</span><span class="sxs-lookup"><span data-stu-id="c5e1c-132">conditions</span></span>|[<span data-ttu-id="c5e1c-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="c5e1c-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="c5e1c-134">Задает правила, которые должны выполняться для применения политики.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="c5e1c-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-135">Required.</span></span> |
|<span data-ttu-id="c5e1c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e1c-136">createdDateTime</span></span>|<span data-ttu-id="c5e1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e1c-137">DateTimeOffset</span></span>| <span data-ttu-id="c5e1c-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c5e1c-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5e1c-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c5e1c-140">Статического.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-140">Readonly.</span></span> |
|<span data-ttu-id="c5e1c-141">description</span><span class="sxs-lookup"><span data-stu-id="c5e1c-141">description</span></span>|<span data-ttu-id="c5e1c-142">String</span><span class="sxs-lookup"><span data-stu-id="c5e1c-142">String</span></span>| <span data-ttu-id="c5e1c-143">Не используется.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-143">Not used.</span></span> |
|<span data-ttu-id="c5e1c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e1c-144">displayName</span></span>|<span data-ttu-id="c5e1c-145">String</span><span class="sxs-lookup"><span data-stu-id="c5e1c-145">String</span></span>| <span data-ttu-id="c5e1c-146">Задает отображаемое имя для объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="c5e1c-147">грантконтролс</span><span class="sxs-lookup"><span data-stu-id="c5e1c-147">grantControls</span></span>|[<span data-ttu-id="c5e1c-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="c5e1c-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="c5e1c-149">Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="c5e1c-150">id</span><span class="sxs-lookup"><span data-stu-id="c5e1c-150">id</span></span>|<span data-ttu-id="c5e1c-151">String</span><span class="sxs-lookup"><span data-stu-id="c5e1c-151">String</span></span>| <span data-ttu-id="c5e1c-152">Задает идентификатор объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="c5e1c-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-153">Read-only.</span></span>|
|<span data-ttu-id="c5e1c-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e1c-154">modifiedDateTime</span></span>| <span data-ttu-id="c5e1c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e1c-155">DateTimeOffset</span></span>|<span data-ttu-id="c5e1c-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c5e1c-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5e1c-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c5e1c-158">Статического.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-158">Readonly.</span></span> |
|<span data-ttu-id="c5e1c-159">сессионконтролс</span><span class="sxs-lookup"><span data-stu-id="c5e1c-159">sessionControls</span></span>|[<span data-ttu-id="c5e1c-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="c5e1c-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="c5e1c-161">Задает элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="c5e1c-162">состояние</span><span class="sxs-lookup"><span data-stu-id="c5e1c-162">state</span></span>|<span data-ttu-id="c5e1c-163">string</span><span class="sxs-lookup"><span data-stu-id="c5e1c-163">string</span></span>| <span data-ttu-id="c5e1c-164">Задает состояние объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="c5e1c-165">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="c5e1c-166">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c5e1c-167">Связи</span><span class="sxs-lookup"><span data-stu-id="c5e1c-167">Relationships</span></span>

<span data-ttu-id="c5e1c-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5e1c-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5e1c-169">JSON representation</span></span>

<span data-ttu-id="c5e1c-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5e1c-170">The following is a JSON representation of the resource.</span></span>

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