---
title: тип ресурса governanceRoleSetting
description: Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: cdc2889624dd9b23920c5cd04ed2c41344cb951c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722288"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="80642-103">тип ресурса governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="80642-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="80642-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80642-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80642-105">Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях.</span><span class="sxs-lookup"><span data-stu-id="80642-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="80642-106">Например, параметры ролей могут включать правило "максимальная продолжительность назначения", правило "MFA, требуемая для активации" и так далее.</span><span class="sxs-lookup"><span data-stu-id="80642-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="80642-107">Методы</span><span class="sxs-lookup"><span data-stu-id="80642-107">Methods</span></span>

| <span data-ttu-id="80642-108">Метод</span><span class="sxs-lookup"><span data-stu-id="80642-108">Method</span></span>          | <span data-ttu-id="80642-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80642-109">Return Type</span></span> |<span data-ttu-id="80642-110">Описание</span><span class="sxs-lookup"><span data-stu-id="80642-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="80642-111">Список</span><span class="sxs-lookup"><span data-stu-id="80642-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="80642-112">[коллекция governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="80642-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="80642-113">Список параметров ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="80642-113">List a collection of role settings on a resource.</span></span>|
|<span data-ttu-id="80642-114">[получение](../api/governancerolesetting-get.md);</span><span class="sxs-lookup"><span data-stu-id="80642-114">[Get](../api/governancerolesetting-get.md)</span></span> |  [<span data-ttu-id="80642-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="80642-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="80642-116">Чтение свойств и связей параметра ролей.</span><span class="sxs-lookup"><span data-stu-id="80642-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="80642-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="80642-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="80642-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="80642-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="80642-119">Обновление объекта параметра роли.</span><span class="sxs-lookup"><span data-stu-id="80642-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80642-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="80642-120">Properties</span></span>
|<span data-ttu-id="80642-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="80642-121">Property</span></span>               |<span data-ttu-id="80642-122">Тип</span><span class="sxs-lookup"><span data-stu-id="80642-122">Type</span></span>                                      |<span data-ttu-id="80642-123">Описание</span><span class="sxs-lookup"><span data-stu-id="80642-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="80642-124">id</span><span class="sxs-lookup"><span data-stu-id="80642-124">id</span></span>                   |<span data-ttu-id="80642-125">String</span><span class="sxs-lookup"><span data-stu-id="80642-125">String</span></span>                                  |<span data-ttu-id="80642-126">Id of the roleSetting.</span><span class="sxs-lookup"><span data-stu-id="80642-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="80642-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="80642-127">resourceId</span></span>           |<span data-ttu-id="80642-128">String</span><span class="sxs-lookup"><span data-stu-id="80642-128">String</span></span>                                  |<span data-ttu-id="80642-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80642-129">Required.</span></span> <span data-ttu-id="80642-130">ID ресурса, с который связан параметр роли.</span><span class="sxs-lookup"><span data-stu-id="80642-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="80642-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="80642-131">roleDefinitionId</span></span>     |<span data-ttu-id="80642-132">String</span><span class="sxs-lookup"><span data-stu-id="80642-132">String</span></span>                                  |<span data-ttu-id="80642-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80642-133">Required.</span></span> <span data-ttu-id="80642-134">ID определения роли, с чем связан параметр роли.</span><span class="sxs-lookup"><span data-stu-id="80642-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="80642-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="80642-135">isDefault</span></span>            |<span data-ttu-id="80642-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="80642-136">Boolean</span></span>                                 |<span data-ttu-id="80642-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80642-137">Read-only.</span></span> <span data-ttu-id="80642-138">Указать, является ли рольSetting ролью по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="80642-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="80642-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="80642-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="80642-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80642-140">DateTimeOffset</span></span>                          |<span data-ttu-id="80642-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80642-141">Read-only.</span></span> <span data-ttu-id="80642-142">Время последнего обновления параметра роли.</span><span class="sxs-lookup"><span data-stu-id="80642-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="80642-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="80642-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80642-144">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="80642-144">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="80642-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="80642-145">lastUpdatedBy</span></span>        |<span data-ttu-id="80642-146">String</span><span class="sxs-lookup"><span data-stu-id="80642-146">String</span></span>                                  |<span data-ttu-id="80642-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80642-147">Read-only.</span></span> <span data-ttu-id="80642-148">Отображает имя администратора, который в последний раз обновлял рольSetting.</span><span class="sxs-lookup"><span data-stu-id="80642-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="80642-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="80642-149">adminEligibleSettings</span></span>|<span data-ttu-id="80642-150">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="80642-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="80642-151">Параметры правил, которые оцениваются при добавлении администратором назначения подходящих ролей.</span><span class="sxs-lookup"><span data-stu-id="80642-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="80642-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="80642-152">adminMemberSettings</span></span>  |<span data-ttu-id="80642-153">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="80642-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="80642-154">Параметры правил, которые оцениваются, когда администратор пытается добавить назначение ролей прямого участника.</span><span class="sxs-lookup"><span data-stu-id="80642-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="80642-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="80642-155">userEligibleSettings</span></span> |<span data-ttu-id="80642-156">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="80642-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="80642-157">Параметры правил, оцениваемые при добавлении права на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="80642-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="80642-158">Параметр пока не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80642-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="80642-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="80642-159">userMemberSettings</span></span>   |<span data-ttu-id="80642-160">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="80642-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="80642-161">Параметры правил, которые оцениваются при попытках пользователя активировать назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="80642-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80642-162">Связи</span><span class="sxs-lookup"><span data-stu-id="80642-162">Relationships</span></span>
| <span data-ttu-id="80642-163">Связь</span><span class="sxs-lookup"><span data-stu-id="80642-163">Relationship</span></span> | <span data-ttu-id="80642-164">Тип</span><span class="sxs-lookup"><span data-stu-id="80642-164">Type</span></span>   |<span data-ttu-id="80642-165">Описание</span><span class="sxs-lookup"><span data-stu-id="80642-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80642-166">resource</span><span class="sxs-lookup"><span data-stu-id="80642-166">resource</span></span>|[<span data-ttu-id="80642-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="80642-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="80642-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80642-168">Read-only.</span></span> <span data-ttu-id="80642-169">Связанный ресурс для этого параметра ролей.</span><span class="sxs-lookup"><span data-stu-id="80642-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="80642-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="80642-170">roleDefinition</span></span>|[<span data-ttu-id="80642-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="80642-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="80642-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80642-172">Read-only.</span></span> <span data-ttu-id="80642-173">Определение роли, которое выполняется с помощью этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="80642-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="80642-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80642-174">JSON representation</span></span>

<span data-ttu-id="80642-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80642-175">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
  "suppressions": []
}
-->


