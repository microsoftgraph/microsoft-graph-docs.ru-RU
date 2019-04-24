---
title: Тип ресурса Говернанцеролесеттинг
description: " и т. д."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506321"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="03787-103">Тип ресурса Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="03787-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03787-104">Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="03787-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="03787-105">Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.</span><span class="sxs-lookup"><span data-stu-id="03787-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="03787-106">Методы</span><span class="sxs-lookup"><span data-stu-id="03787-106">Methods</span></span>

| <span data-ttu-id="03787-107">Метод</span><span class="sxs-lookup"><span data-stu-id="03787-107">Method</span></span>          | <span data-ttu-id="03787-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03787-108">Return Type</span></span> |<span data-ttu-id="03787-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03787-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="03787-110">List</span><span class="sxs-lookup"><span data-stu-id="03787-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="03787-111">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="03787-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="03787-112">ПереЧисление коллекции параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="03787-112">List a collection of role settings on a resource.</span></span>|
|<span data-ttu-id="03787-113">[получение](../api/governancerolesetting-get.md);</span><span class="sxs-lookup"><span data-stu-id="03787-113">[Get](../api/governancerolesetting-get.md)</span></span> |  [<span data-ttu-id="03787-114">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="03787-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="03787-115">Чтение свойств и связей параметра Role.</span><span class="sxs-lookup"><span data-stu-id="03787-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="03787-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="03787-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="03787-117">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="03787-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="03787-118">Обновление объекта параметров роли.</span><span class="sxs-lookup"><span data-stu-id="03787-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="03787-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="03787-119">Properties</span></span>
|<span data-ttu-id="03787-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="03787-120">Property</span></span>               |<span data-ttu-id="03787-121">Тип</span><span class="sxs-lookup"><span data-stu-id="03787-121">Type</span></span>                                      |<span data-ttu-id="03787-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03787-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="03787-123">id</span><span class="sxs-lookup"><span data-stu-id="03787-123">id</span></span>                   |<span data-ttu-id="03787-124">String</span><span class="sxs-lookup"><span data-stu-id="03787-124">String</span></span>                                  |<span data-ttu-id="03787-125">Идентификатор Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="03787-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="03787-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="03787-126">resourceId</span></span>           |<span data-ttu-id="03787-127">String</span><span class="sxs-lookup"><span data-stu-id="03787-127">String</span></span>                                  |<span data-ttu-id="03787-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03787-128">Required.</span></span> <span data-ttu-id="03787-129">Идентификатор ресурса, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="03787-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="03787-130">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="03787-130">roleDefinitionId</span></span>     |<span data-ttu-id="03787-131">String</span><span class="sxs-lookup"><span data-stu-id="03787-131">String</span></span>                                  |<span data-ttu-id="03787-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03787-132">Required.</span></span> <span data-ttu-id="03787-133">Идентификатор определения роли, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="03787-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="03787-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="03787-134">isDefault</span></span>            |<span data-ttu-id="03787-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="03787-135">Boolean</span></span>                                 |<span data-ttu-id="03787-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03787-136">Read-only.</span></span> <span data-ttu-id="03787-137">Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="03787-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="03787-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="03787-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="03787-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03787-139">DateTimeOffset</span></span>                          |<span data-ttu-id="03787-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03787-140">Read-only.</span></span> <span data-ttu-id="03787-141">Время последнего обновления параметра роли.</span><span class="sxs-lookup"><span data-stu-id="03787-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="03787-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="03787-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03787-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03787-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="03787-144">Ластупдатедби</span><span class="sxs-lookup"><span data-stu-id="03787-144">lastUpdatedBy</span></span>        |<span data-ttu-id="03787-145">String</span><span class="sxs-lookup"><span data-stu-id="03787-145">String</span></span>                                  |<span data-ttu-id="03787-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03787-146">Read-only.</span></span> <span data-ttu-id="03787-147">Отображаемое имя администратора, который последним обновил Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="03787-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="03787-148">Админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="03787-148">adminEligibleSettings</span></span>|<span data-ttu-id="03787-149">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="03787-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="03787-150">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="03787-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="03787-151">Админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="03787-151">adminMemberSettings</span></span>  |<span data-ttu-id="03787-152">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="03787-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="03787-153">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="03787-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="03787-154">Усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="03787-154">userEligibleSettings</span></span> |<span data-ttu-id="03787-155">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="03787-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="03787-156">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="03787-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="03787-157">Этот параметр не поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="03787-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="03787-158">Усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="03787-158">userMemberSettings</span></span>   |<span data-ttu-id="03787-159">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="03787-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="03787-160">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="03787-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03787-161">Связи</span><span class="sxs-lookup"><span data-stu-id="03787-161">Relationships</span></span>
| <span data-ttu-id="03787-162">Отношение</span><span class="sxs-lookup"><span data-stu-id="03787-162">Relationship</span></span> | <span data-ttu-id="03787-163">Тип</span><span class="sxs-lookup"><span data-stu-id="03787-163">Type</span></span>   |<span data-ttu-id="03787-164">Описание</span><span class="sxs-lookup"><span data-stu-id="03787-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03787-165">resource</span><span class="sxs-lookup"><span data-stu-id="03787-165">resource</span></span>|[<span data-ttu-id="03787-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="03787-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="03787-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03787-167">Read-only.</span></span> <span data-ttu-id="03787-168">Связанный ресурс для этого параметра Role.</span><span class="sxs-lookup"><span data-stu-id="03787-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="03787-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="03787-169">roleDefinition</span></span>|[<span data-ttu-id="03787-170">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="03787-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="03787-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03787-171">Read-only.</span></span> <span data-ttu-id="03787-172">Определение роли, принудительно заданное с помощью этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="03787-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03787-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03787-173">JSON representation</span></span>

<span data-ttu-id="03787-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03787-174">Here is a JSON representation of the resource.</span></span>

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
