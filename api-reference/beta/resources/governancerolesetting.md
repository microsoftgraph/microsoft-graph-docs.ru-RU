---
title: Тип ресурса governanceRoleSetting
description: " правила и т. д."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508169"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="fe70a-103">Тип ресурса governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="fe70a-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe70a-104">Представляет набор конфигураций на каждое определение роли, которое должно использоваться для вычисления при создании или измененные назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="fe70a-105">К примеру параметры роли могут содержать правила «назначения Максимальная длительность», «Многофакторной проверкой Подлинности требуется на активации» правила и т.д.</span><span class="sxs-lookup"><span data-stu-id="fe70a-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="fe70a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fe70a-106">Methods</span></span>

| <span data-ttu-id="fe70a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fe70a-107">Method</span></span>          | <span data-ttu-id="fe70a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe70a-108">Return Type</span></span> |<span data-ttu-id="fe70a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fe70a-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="fe70a-110">List</span><span class="sxs-lookup"><span data-stu-id="fe70a-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="fe70a-111">[governanceRoleSetting](../resources/governancerolesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe70a-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="fe70a-112">Список коллекцию параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="fe70a-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="fe70a-113">Get</span><span class="sxs-lookup"><span data-stu-id="fe70a-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="fe70a-114">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="fe70a-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="fe70a-115">Чтение свойства и связи параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="fe70a-116">Update</span><span class="sxs-lookup"><span data-stu-id="fe70a-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="fe70a-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="fe70a-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="fe70a-118">Обновите объект параметров роли.</span><span class="sxs-lookup"><span data-stu-id="fe70a-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe70a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe70a-119">Properties</span></span>
|<span data-ttu-id="fe70a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe70a-120">Property</span></span>               |<span data-ttu-id="fe70a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fe70a-121">Type</span></span>                                      |<span data-ttu-id="fe70a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fe70a-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="fe70a-123">id</span><span class="sxs-lookup"><span data-stu-id="fe70a-123">id</span></span>                   |<span data-ttu-id="fe70a-124">String</span><span class="sxs-lookup"><span data-stu-id="fe70a-124">String</span></span>                                  |<span data-ttu-id="fe70a-125">Идентификатор roleSetting.</span><span class="sxs-lookup"><span data-stu-id="fe70a-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="fe70a-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="fe70a-126">resourceId</span></span>           |<span data-ttu-id="fe70a-127">String</span><span class="sxs-lookup"><span data-stu-id="fe70a-127">String</span></span>                                  |<span data-ttu-id="fe70a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe70a-128">Required.</span></span> <span data-ttu-id="fe70a-129">Идентификатор ресурса, с которым связана параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="fe70a-130">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fe70a-130">roleDefinitionId</span></span>     |<span data-ttu-id="fe70a-131">Строка</span><span class="sxs-lookup"><span data-stu-id="fe70a-131">String</span></span>                                  |<span data-ttu-id="fe70a-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe70a-132">Required.</span></span> <span data-ttu-id="fe70a-133">Идентификатор определения роли, с которым связана параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="fe70a-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="fe70a-134">isDefault</span></span>            |<span data-ttu-id="fe70a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe70a-135">Boolean</span></span>                                 |<span data-ttu-id="fe70a-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe70a-136">Read-only.</span></span> <span data-ttu-id="fe70a-137">Укажите, является ли roleSetting roleSetting по умолчанию</span><span class="sxs-lookup"><span data-stu-id="fe70a-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="fe70a-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe70a-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="fe70a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe70a-139">DateTimeOffset</span></span>                          |<span data-ttu-id="fe70a-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe70a-140">Read-only.</span></span> <span data-ttu-id="fe70a-141">Время последнего обновления параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="fe70a-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fe70a-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe70a-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fe70a-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fe70a-144">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="fe70a-144">lastUpdatedBy</span></span>        |<span data-ttu-id="fe70a-145">String</span><span class="sxs-lookup"><span data-stu-id="fe70a-145">String</span></span>                                  |<span data-ttu-id="fe70a-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe70a-146">Read-only.</span></span> <span data-ttu-id="fe70a-147">Отображаемое имя администратора, который последним обновил roleSetting.</span><span class="sxs-lookup"><span data-stu-id="fe70a-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="fe70a-148">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="fe70a-148">adminEligibleSettings</span></span>|<span data-ttu-id="fe70a-149">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe70a-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fe70a-150">Параметры правил, которые вычисляются, когда администратор пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="fe70a-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="fe70a-151">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="fe70a-151">adminMemberSettings</span></span>  |<span data-ttu-id="fe70a-152">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe70a-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fe70a-153">Параметры правил, которые вычисляются, когда администратор пытается добавить членами назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="fe70a-154">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="fe70a-154">userEligibleSettings</span></span> |<span data-ttu-id="fe70a-155">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe70a-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fe70a-156">Параметры правил, которые вычисляются, когда пользователь пытается добавить назначение подходящими роли.</span><span class="sxs-lookup"><span data-stu-id="fe70a-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="fe70a-157">Параметр не поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="fe70a-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="fe70a-158">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="fe70a-158">userMemberSettings</span></span>   |<span data-ttu-id="fe70a-159">[governanceRuleSetting](../resources/governancerulesetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe70a-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="fe70a-160">Параметры правил, которые вычисляются при попытке активировать его назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fe70a-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe70a-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="fe70a-161">Relationships</span></span>
| <span data-ttu-id="fe70a-162">Связь</span><span class="sxs-lookup"><span data-stu-id="fe70a-162">Relationship</span></span> | <span data-ttu-id="fe70a-163">Тип</span><span class="sxs-lookup"><span data-stu-id="fe70a-163">Type</span></span>   |<span data-ttu-id="fe70a-164">Описание</span><span class="sxs-lookup"><span data-stu-id="fe70a-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe70a-165">resource</span><span class="sxs-lookup"><span data-stu-id="fe70a-165">resource</span></span>|[<span data-ttu-id="fe70a-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="fe70a-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="fe70a-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe70a-167">Read-only.</span></span> <span data-ttu-id="fe70a-168">Связанные ресурсов для этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="fe70a-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="fe70a-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fe70a-169">roleDefinition</span></span>|[<span data-ttu-id="fe70a-170">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="fe70a-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="fe70a-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe70a-171">Read-only.</span></span> <span data-ttu-id="fe70a-172">Определение роли, которое применяется при использовании этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="fe70a-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe70a-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe70a-173">JSON representation</span></span>

<span data-ttu-id="fe70a-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe70a-174">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
