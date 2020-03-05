---
title: Тип ресурса Кондитионалакцессполици
description: Представляет политику условного доступа Azure Active Directory. Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: baa5daded03e9ddc5dedbb97f86d15d690240d09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507529"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="8f467-104">Тип ресурса Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="8f467-104">conditionalAccessPolicy resource type</span></span>

<span data-ttu-id="8f467-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8f467-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f467-106">Представляет политику условного доступа Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8f467-106">Represents an Azure Active Directory conditional access policy.</span></span> <span data-ttu-id="8f467-107">Политики условного доступа — это настраиваемые правила, определяющие сценарий доступа.</span><span class="sxs-lookup"><span data-stu-id="8f467-107">Conditional access policies are custom rules that define an access scenario.</span></span> <span data-ttu-id="8f467-108">Дополнительные сведения см. в [документации по условному доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="8f467-108">For more information, see the [Conditional access documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>

## <a name="methods"></a><span data-ttu-id="8f467-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8f467-109">Methods</span></span>

| <span data-ttu-id="8f467-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8f467-110">Method</span></span>       | <span data-ttu-id="8f467-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f467-111">Return Type</span></span> | <span data-ttu-id="8f467-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8f467-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8f467-113">Список КондитионалакцессполиЦиес</span><span class="sxs-lookup"><span data-stu-id="8f467-113">List conditionalAccessPolicies</span></span>](../api/conditionalaccessroot-list-policies.md) | <span data-ttu-id="8f467-114">Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-114">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span> | <span data-ttu-id="8f467-115">Получение всех объектов КондитионалакцессполиЦиес в Организации.</span><span class="sxs-lookup"><span data-stu-id="8f467-115">Get all of the conditionalAccessPolicies objects in the organization.</span></span> |
| [<span data-ttu-id="8f467-116">Создание Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="8f467-116">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) | [<span data-ttu-id="8f467-117">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8f467-117">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="8f467-118">Создание нового объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-118">Create a new conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="8f467-119">Получение Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="8f467-119">Get conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-get.md) | [<span data-ttu-id="8f467-120">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8f467-120">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="8f467-121">Чтение свойств и связей объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-121">Read properties and relationships of a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="8f467-122">Обновление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="8f467-122">Update conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-update.md) | [<span data-ttu-id="8f467-123">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8f467-123">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md) | <span data-ttu-id="8f467-124">Обновление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-124">Update a conditionalAccessPolicy object.</span></span> |
| [<span data-ttu-id="8f467-125">Удаление Кондитионалакцессполици</span><span class="sxs-lookup"><span data-stu-id="8f467-125">Delete conditionalAccessPolicy</span></span>](../api/conditionalaccesspolicy-delete.md) | <span data-ttu-id="8f467-126">Нет</span><span class="sxs-lookup"><span data-stu-id="8f467-126">None</span></span> | <span data-ttu-id="8f467-127">Удаление объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-127">Delete a conditionalAccessPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f467-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f467-128">Properties</span></span>

| <span data-ttu-id="8f467-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f467-129">Property</span></span>     | <span data-ttu-id="8f467-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f467-130">Type</span></span>        | <span data-ttu-id="8f467-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f467-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f467-132">conditions</span><span class="sxs-lookup"><span data-stu-id="8f467-132">conditions</span></span>|[<span data-ttu-id="8f467-133">conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="8f467-133">conditionalAccessConditionSet</span></span>](conditionalaccessconditionset.md)| <span data-ttu-id="8f467-134">Задает правила, которые должны выполняться для применения политики.</span><span class="sxs-lookup"><span data-stu-id="8f467-134">Specifies the rules that must be met for the policy to apply.</span></span> <span data-ttu-id="8f467-135">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8f467-135">Required.</span></span> |
|<span data-ttu-id="8f467-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f467-136">createdDateTime</span></span>|<span data-ttu-id="8f467-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f467-137">DateTimeOffset</span></span>| <span data-ttu-id="8f467-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8f467-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f467-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8f467-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8f467-140">Статического.</span><span class="sxs-lookup"><span data-stu-id="8f467-140">Readonly.</span></span> |
|<span data-ttu-id="8f467-141">description</span><span class="sxs-lookup"><span data-stu-id="8f467-141">description</span></span>|<span data-ttu-id="8f467-142">String</span><span class="sxs-lookup"><span data-stu-id="8f467-142">String</span></span>| <span data-ttu-id="8f467-143">Не используется.</span><span class="sxs-lookup"><span data-stu-id="8f467-143">Not used.</span></span> |
|<span data-ttu-id="8f467-144">displayName</span><span class="sxs-lookup"><span data-stu-id="8f467-144">displayName</span></span>|<span data-ttu-id="8f467-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8f467-145">String</span></span>| <span data-ttu-id="8f467-146">Задает отображаемое имя для объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-146">Specifies a display name for the conditionalAccessPolicy object.</span></span> |
|<span data-ttu-id="8f467-147">грантконтролс</span><span class="sxs-lookup"><span data-stu-id="8f467-147">grantControls</span></span>|[<span data-ttu-id="8f467-148">conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="8f467-148">conditionalAccessGrantControls</span></span>](conditionalaccessgrantcontrols.md)| <span data-ttu-id="8f467-149">Указывает элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="8f467-149">Specifies the grant controls that must be fulfilled to pass the policy.</span></span> |
|<span data-ttu-id="8f467-150">id</span><span class="sxs-lookup"><span data-stu-id="8f467-150">id</span></span>|<span data-ttu-id="8f467-151">String</span><span class="sxs-lookup"><span data-stu-id="8f467-151">String</span></span>| <span data-ttu-id="8f467-152">Задает идентификатор объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-152">Specifies the identifier of a conditionalAccessPolicy object.</span></span> <span data-ttu-id="8f467-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f467-153">Read-only.</span></span>|
|<span data-ttu-id="8f467-154">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f467-154">modifiedDateTime</span></span>| <span data-ttu-id="8f467-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f467-155">DateTimeOffset</span></span>|<span data-ttu-id="8f467-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8f467-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f467-157">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8f467-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8f467-158">Статического.</span><span class="sxs-lookup"><span data-stu-id="8f467-158">Readonly.</span></span> |
|<span data-ttu-id="8f467-159">сессионконтролс</span><span class="sxs-lookup"><span data-stu-id="8f467-159">sessionControls</span></span>|[<span data-ttu-id="8f467-160">conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="8f467-160">conditionalAccessSessionControls</span></span>](conditionalaccesssessioncontrols.md)| <span data-ttu-id="8f467-161">Задает элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="8f467-161">Specifies the session controls that are enforced after sign-in.</span></span> |
|<span data-ttu-id="8f467-162">состояние</span><span class="sxs-lookup"><span data-stu-id="8f467-162">state</span></span>|<span data-ttu-id="8f467-163">строка</span><span class="sxs-lookup"><span data-stu-id="8f467-163">string</span></span>| <span data-ttu-id="8f467-164">Задает состояние объекта Кондитионалакцессполици.</span><span class="sxs-lookup"><span data-stu-id="8f467-164">Specifies the state of the conditionalAccessPolicy object.</span></span> <span data-ttu-id="8f467-165">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="8f467-165">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="8f467-166">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="8f467-166">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f467-167">Связи</span><span class="sxs-lookup"><span data-stu-id="8f467-167">Relationships</span></span>

<span data-ttu-id="8f467-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8f467-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f467-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8f467-169">JSON representation</span></span>

<span data-ttu-id="8f467-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f467-170">The following is a JSON representation of the resource.</span></span>

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
