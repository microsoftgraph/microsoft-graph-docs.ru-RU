---
title: Тип ресурса governanceRoleSetting
description: " правила и т. д."
ms.openlocfilehash: 64245b2d6f0aa9e0ea3ffda4a5eaebfb9fd205df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079099"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="bfb9d-103">Тип ресурса governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfb9d-103">governanceRoleSetting resource type</span></span>

> <span data-ttu-id="bfb9d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfb9d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfb9d-106">Представляет набор конфигураций на каждое определение роли, которое должно использоваться для вычисления при создании или измененные назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-106">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="bfb9d-107">К примеру параметры роли могут содержать правила «назначения Максимальная длительность», «Многофакторной проверкой Подлинности требуется на активации» правила и т.д.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-107">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="bfb9d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bfb9d-108">Methods</span></span>

| <span data-ttu-id="bfb9d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bfb9d-109">Method</span></span>          | <span data-ttu-id="bfb9d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bfb9d-110">Return Type</span></span> |<span data-ttu-id="bfb9d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb9d-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="bfb9d-112">List</span><span class="sxs-lookup"><span data-stu-id="bfb9d-112">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="bfb9d-113">[governanceRoleSetting](../resources/governancerolesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bfb9d-113">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="bfb9d-114">Список коллекцию параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-114">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="bfb9d-115">Get</span><span class="sxs-lookup"><span data-stu-id="bfb9d-115">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="bfb9d-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfb9d-116">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="bfb9d-117">Чтение свойства и связи параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-117">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="bfb9d-118">Update</span><span class="sxs-lookup"><span data-stu-id="bfb9d-118">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="bfb9d-119">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bfb9d-119">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="bfb9d-120">Обновите объект параметров роли.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-120">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfb9d-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfb9d-121">Properties</span></span>
|<span data-ttu-id="bfb9d-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfb9d-122">Property</span></span>               |<span data-ttu-id="bfb9d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bfb9d-123">Type</span></span>                                      |<span data-ttu-id="bfb9d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb9d-124">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="bfb9d-125">id</span><span class="sxs-lookup"><span data-stu-id="bfb9d-125">id</span></span>                   |<span data-ttu-id="bfb9d-126">String</span><span class="sxs-lookup"><span data-stu-id="bfb9d-126">String</span></span>                                  |<span data-ttu-id="bfb9d-127">Идентификатор roleSetting.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-127">The id of the roleSetting.</span></span>|
|<span data-ttu-id="bfb9d-128">resourceId</span><span class="sxs-lookup"><span data-stu-id="bfb9d-128">resourceId</span></span>           |<span data-ttu-id="bfb9d-129">String</span><span class="sxs-lookup"><span data-stu-id="bfb9d-129">String</span></span>                                  |<span data-ttu-id="bfb9d-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-130">Required.</span></span> <span data-ttu-id="bfb9d-131">Идентификатор ресурса, с которым связана параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-131">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="bfb9d-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="bfb9d-132">roleDefinitionId</span></span>     |<span data-ttu-id="bfb9d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bfb9d-133">String</span></span>                                  |<span data-ttu-id="bfb9d-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-134">Required.</span></span> <span data-ttu-id="bfb9d-135">Идентификатор определения роли, с которым связана параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-135">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="bfb9d-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="bfb9d-136">isDefault</span></span>            |<span data-ttu-id="bfb9d-137">Логический</span><span class="sxs-lookup"><span data-stu-id="bfb9d-137">Boolean</span></span>                                 |<span data-ttu-id="bfb9d-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-138">Read-only.</span></span> <span data-ttu-id="bfb9d-139">Укажите, является ли roleSetting roleSetting по умолчанию</span><span class="sxs-lookup"><span data-stu-id="bfb9d-139">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="bfb9d-140">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfb9d-140">lastUpdatedDateTime</span></span>  |<span data-ttu-id="bfb9d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfb9d-141">DateTimeOffset</span></span>                          |<span data-ttu-id="bfb9d-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-142">Read-only.</span></span> <span data-ttu-id="bfb9d-143">Время последнего обновления параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-143">The time when the role setting was last updated.</span></span> <span data-ttu-id="bfb9d-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bfb9d-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfb9d-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfb9d-146">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="bfb9d-146">lastUpdatedBy</span></span>        |<span data-ttu-id="bfb9d-147">String</span><span class="sxs-lookup"><span data-stu-id="bfb9d-147">String</span></span>                                  |<span data-ttu-id="bfb9d-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-148">Read-only.</span></span> <span data-ttu-id="bfb9d-149">Отображаемое имя администратора, который последним обновил roleSetting.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-149">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="bfb9d-150">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bfb9d-150">adminEligibleSettings</span></span>|<span data-ttu-id="bfb9d-151">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bfb9d-151">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfb9d-152">Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-152">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="bfb9d-153">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bfb9d-153">adminMemberSettings</span></span>  |<span data-ttu-id="bfb9d-154">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bfb9d-154">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfb9d-155">Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-155">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="bfb9d-156">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bfb9d-156">userEligibleSettings</span></span> |<span data-ttu-id="bfb9d-157">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bfb9d-157">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfb9d-158">Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-158">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="bfb9d-159">Параметр не поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-159">The setting is not supported for now.</span></span>|
|<span data-ttu-id="bfb9d-160">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bfb9d-160">userMemberSettings</span></span>   |<span data-ttu-id="bfb9d-161">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bfb9d-161">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bfb9d-162">Параметры правил, которые вычисляются при попытке активировать его назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-162">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb9d-163">Связи</span><span class="sxs-lookup"><span data-stu-id="bfb9d-163">Relationships</span></span>
| <span data-ttu-id="bfb9d-164">Связь</span><span class="sxs-lookup"><span data-stu-id="bfb9d-164">Relationship</span></span> | <span data-ttu-id="bfb9d-165">Тип</span><span class="sxs-lookup"><span data-stu-id="bfb9d-165">Type</span></span>   |<span data-ttu-id="bfb9d-166">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb9d-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb9d-167">resource</span><span class="sxs-lookup"><span data-stu-id="bfb9d-167">resource</span></span>|[<span data-ttu-id="bfb9d-168">governanceResource</span><span class="sxs-lookup"><span data-stu-id="bfb9d-168">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="bfb9d-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-169">Read-only.</span></span> <span data-ttu-id="bfb9d-170">Связанные ресурсов для этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-170">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="bfb9d-171">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bfb9d-171">roleDefinition</span></span>|[<span data-ttu-id="bfb9d-172">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bfb9d-172">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="bfb9d-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-173">Read-only.</span></span> <span data-ttu-id="bfb9d-174">Определение роли, которое применяется при использовании этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-174">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfb9d-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfb9d-175">JSON representation</span></span>

<span data-ttu-id="bfb9d-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfb9d-176">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
