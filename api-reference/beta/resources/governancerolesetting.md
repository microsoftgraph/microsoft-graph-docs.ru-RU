---
title: тип ресурса governanceRoleSetting
description: Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 414ccfcea47892e1d9479771ffd7b1dea8b77770
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440313"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="76ee7-103">тип ресурса governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="76ee7-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="76ee7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76ee7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76ee7-105">Представляет набор конфигураций для каждого определения ролей, которые необходимо оценивать при назначении ролей при их назначении или изменениях.</span><span class="sxs-lookup"><span data-stu-id="76ee7-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="76ee7-106">Например, параметры ролей могут включать правило "максимальная продолжительность назначения", правило "MFA, требуемая для активации" и так далее.</span><span class="sxs-lookup"><span data-stu-id="76ee7-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="76ee7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="76ee7-107">Methods</span></span>

| <span data-ttu-id="76ee7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="76ee7-108">Method</span></span>          | <span data-ttu-id="76ee7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="76ee7-109">Return Type</span></span> |<span data-ttu-id="76ee7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76ee7-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="76ee7-111">Список</span><span class="sxs-lookup"><span data-stu-id="76ee7-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="76ee7-112">[коллекция governanceRoleSetting](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="76ee7-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="76ee7-113">Список параметров ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="76ee7-113">List a collection of role settings on a resource.</span></span>|
|<span data-ttu-id="76ee7-114">[получение](../api/governancerolesetting-get.md);</span><span class="sxs-lookup"><span data-stu-id="76ee7-114">[Get](../api/governancerolesetting-get.md)</span></span> |  [<span data-ttu-id="76ee7-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="76ee7-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="76ee7-116">Чтение свойств и связей параметра ролей.</span><span class="sxs-lookup"><span data-stu-id="76ee7-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="76ee7-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="76ee7-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="76ee7-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="76ee7-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="76ee7-119">Обновление объекта параметра роли.</span><span class="sxs-lookup"><span data-stu-id="76ee7-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="76ee7-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="76ee7-120">Properties</span></span>
|<span data-ttu-id="76ee7-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="76ee7-121">Property</span></span>               |<span data-ttu-id="76ee7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="76ee7-122">Type</span></span>                                      |<span data-ttu-id="76ee7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="76ee7-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="76ee7-124">id</span><span class="sxs-lookup"><span data-stu-id="76ee7-124">id</span></span>                   |<span data-ttu-id="76ee7-125">String</span><span class="sxs-lookup"><span data-stu-id="76ee7-125">String</span></span>                                  |<span data-ttu-id="76ee7-126">Id of the roleSetting.</span><span class="sxs-lookup"><span data-stu-id="76ee7-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="76ee7-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="76ee7-127">resourceId</span></span>           |<span data-ttu-id="76ee7-128">String</span><span class="sxs-lookup"><span data-stu-id="76ee7-128">String</span></span>                                  |<span data-ttu-id="76ee7-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76ee7-129">Required.</span></span> <span data-ttu-id="76ee7-130">ID ресурса, с который связан параметр роли.</span><span class="sxs-lookup"><span data-stu-id="76ee7-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="76ee7-131">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="76ee7-131">roleDefinitionId</span></span>     |<span data-ttu-id="76ee7-132">String</span><span class="sxs-lookup"><span data-stu-id="76ee7-132">String</span></span>                                  |<span data-ttu-id="76ee7-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76ee7-133">Required.</span></span> <span data-ttu-id="76ee7-134">ID определения роли, с чем связан параметр роли.</span><span class="sxs-lookup"><span data-stu-id="76ee7-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="76ee7-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="76ee7-135">isDefault</span></span>            |<span data-ttu-id="76ee7-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="76ee7-136">Boolean</span></span>                                 |<span data-ttu-id="76ee7-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76ee7-137">Read-only.</span></span> <span data-ttu-id="76ee7-138">Указать, является ли рольSetting ролью по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="76ee7-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="76ee7-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="76ee7-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="76ee7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76ee7-140">DateTimeOffset</span></span>                          |<span data-ttu-id="76ee7-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76ee7-141">Read-only.</span></span> <span data-ttu-id="76ee7-142">Время последнего обновления параметра роли.</span><span class="sxs-lookup"><span data-stu-id="76ee7-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="76ee7-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="76ee7-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76ee7-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="76ee7-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="76ee7-145">lastUpdatedBy</span><span class="sxs-lookup"><span data-stu-id="76ee7-145">lastUpdatedBy</span></span>        |<span data-ttu-id="76ee7-146">String</span><span class="sxs-lookup"><span data-stu-id="76ee7-146">String</span></span>                                  |<span data-ttu-id="76ee7-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76ee7-147">Read-only.</span></span> <span data-ttu-id="76ee7-148">Отображает имя администратора, который в последний раз обновлял рольSetting.</span><span class="sxs-lookup"><span data-stu-id="76ee7-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="76ee7-149">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="76ee7-149">adminEligibleSettings</span></span>|<span data-ttu-id="76ee7-150">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="76ee7-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="76ee7-151">Параметры правил, которые оцениваются при добавлении администратором назначения подходящих ролей.</span><span class="sxs-lookup"><span data-stu-id="76ee7-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="76ee7-152">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="76ee7-152">adminMemberSettings</span></span>  |<span data-ttu-id="76ee7-153">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="76ee7-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="76ee7-154">Параметры правил, которые оцениваются, когда администратор пытается добавить назначение ролей прямого участника.</span><span class="sxs-lookup"><span data-stu-id="76ee7-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="76ee7-155">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="76ee7-155">userEligibleSettings</span></span> |<span data-ttu-id="76ee7-156">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="76ee7-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="76ee7-157">Параметры правил, оцениваемые при добавлении права на назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="76ee7-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="76ee7-158">Параметр пока не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ee7-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="76ee7-159">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="76ee7-159">userMemberSettings</span></span>   |<span data-ttu-id="76ee7-160">[коллекция governanceRuleSetting](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="76ee7-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="76ee7-161">Параметры правил, которые оцениваются при попытках пользователя активировать назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="76ee7-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76ee7-162">Связи</span><span class="sxs-lookup"><span data-stu-id="76ee7-162">Relationships</span></span>
| <span data-ttu-id="76ee7-163">Связь</span><span class="sxs-lookup"><span data-stu-id="76ee7-163">Relationship</span></span> | <span data-ttu-id="76ee7-164">Тип</span><span class="sxs-lookup"><span data-stu-id="76ee7-164">Type</span></span>   |<span data-ttu-id="76ee7-165">Описание</span><span class="sxs-lookup"><span data-stu-id="76ee7-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76ee7-166">resource</span><span class="sxs-lookup"><span data-stu-id="76ee7-166">resource</span></span>|[<span data-ttu-id="76ee7-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="76ee7-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="76ee7-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76ee7-168">Read-only.</span></span> <span data-ttu-id="76ee7-169">Связанный ресурс для этого параметра ролей.</span><span class="sxs-lookup"><span data-stu-id="76ee7-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="76ee7-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="76ee7-170">roleDefinition</span></span>|[<span data-ttu-id="76ee7-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="76ee7-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="76ee7-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76ee7-172">Read-only.</span></span> <span data-ttu-id="76ee7-173">Определение роли, которое выполняется с помощью этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="76ee7-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76ee7-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76ee7-174">JSON representation</span></span>

<span data-ttu-id="76ee7-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76ee7-175">Here is a JSON representation of the resource.</span></span>

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


