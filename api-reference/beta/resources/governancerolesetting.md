---
title: Тип ресурса Говернанцеролесеттинг
description: " и т. д."
localization_priority: Normal
ms.openlocfilehash: 09e8cb65f8318294d483a2ad66a7119d7b48822a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340233"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="19391-103">Тип ресурса Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="19391-103">governanceRoleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19391-104">Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="19391-104">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="19391-105">Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.</span><span class="sxs-lookup"><span data-stu-id="19391-105">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="19391-106">Методы</span><span class="sxs-lookup"><span data-stu-id="19391-106">Methods</span></span>

| <span data-ttu-id="19391-107">Метод</span><span class="sxs-lookup"><span data-stu-id="19391-107">Method</span></span>          | <span data-ttu-id="19391-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19391-108">Return Type</span></span> |<span data-ttu-id="19391-109">Описание</span><span class="sxs-lookup"><span data-stu-id="19391-109">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="19391-110">Список</span><span class="sxs-lookup"><span data-stu-id="19391-110">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="19391-111">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="19391-111">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="19391-112">ПереЧисление коллекции параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="19391-112">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="19391-113">Получение</span><span class="sxs-lookup"><span data-stu-id="19391-113">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="19391-114">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="19391-114">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="19391-115">Чтение свойств и связей параметра Role.</span><span class="sxs-lookup"><span data-stu-id="19391-115">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="19391-116">Update</span><span class="sxs-lookup"><span data-stu-id="19391-116">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="19391-117">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="19391-117">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="19391-118">Обновление объекта параметров роли.</span><span class="sxs-lookup"><span data-stu-id="19391-118">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="19391-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="19391-119">Properties</span></span>
|<span data-ttu-id="19391-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="19391-120">Property</span></span>               |<span data-ttu-id="19391-121">Тип</span><span class="sxs-lookup"><span data-stu-id="19391-121">Type</span></span>                                      |<span data-ttu-id="19391-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19391-122">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="19391-123">id</span><span class="sxs-lookup"><span data-stu-id="19391-123">id</span></span>                   |<span data-ttu-id="19391-124">Строка</span><span class="sxs-lookup"><span data-stu-id="19391-124">String</span></span>                                  |<span data-ttu-id="19391-125">Идентификатор Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="19391-125">The id of the roleSetting.</span></span>|
|<span data-ttu-id="19391-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="19391-126">resourceId</span></span>           |<span data-ttu-id="19391-127">String</span><span class="sxs-lookup"><span data-stu-id="19391-127">String</span></span>                                  |<span data-ttu-id="19391-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19391-128">Required.</span></span> <span data-ttu-id="19391-129">Идентификатор ресурса, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="19391-129">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="19391-130">Роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="19391-130">roleDefinitionId</span></span>     |<span data-ttu-id="19391-131">String</span><span class="sxs-lookup"><span data-stu-id="19391-131">String</span></span>                                  |<span data-ttu-id="19391-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19391-132">Required.</span></span> <span data-ttu-id="19391-133">Идентификатор определения роли, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="19391-133">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="19391-134">isDefault</span><span class="sxs-lookup"><span data-stu-id="19391-134">isDefault</span></span>            |<span data-ttu-id="19391-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="19391-135">Boolean</span></span>                                 |<span data-ttu-id="19391-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19391-136">Read-only.</span></span> <span data-ttu-id="19391-137">Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="19391-137">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="19391-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="19391-138">lastUpdatedDateTime</span></span>  |<span data-ttu-id="19391-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19391-139">DateTimeOffset</span></span>                          |<span data-ttu-id="19391-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19391-140">Read-only.</span></span> <span data-ttu-id="19391-141">Время последнего обновления параметра роли.</span><span class="sxs-lookup"><span data-stu-id="19391-141">The time when the role setting was last updated.</span></span> <span data-ttu-id="19391-142">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="19391-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="19391-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="19391-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="19391-144">Ластупдатедби</span><span class="sxs-lookup"><span data-stu-id="19391-144">lastUpdatedBy</span></span>        |<span data-ttu-id="19391-145">String</span><span class="sxs-lookup"><span data-stu-id="19391-145">String</span></span>                                  |<span data-ttu-id="19391-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19391-146">Read-only.</span></span> <span data-ttu-id="19391-147">Отображаемое имя администратора, который последним обновил Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="19391-147">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="19391-148">Админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="19391-148">adminEligibleSettings</span></span>|<span data-ttu-id="19391-149">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="19391-149">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="19391-150">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="19391-150">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="19391-151">Админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="19391-151">adminMemberSettings</span></span>  |<span data-ttu-id="19391-152">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="19391-152">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="19391-153">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="19391-153">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="19391-154">Усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="19391-154">userEligibleSettings</span></span> |<span data-ttu-id="19391-155">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="19391-155">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="19391-156">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="19391-156">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="19391-157">Этот параметр не поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="19391-157">The setting is not supported for now.</span></span>|
|<span data-ttu-id="19391-158">Усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="19391-158">userMemberSettings</span></span>   |<span data-ttu-id="19391-159">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="19391-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="19391-160">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="19391-160">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19391-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="19391-161">Relationships</span></span>
| <span data-ttu-id="19391-162">Отношение</span><span class="sxs-lookup"><span data-stu-id="19391-162">Relationship</span></span> | <span data-ttu-id="19391-163">Тип</span><span class="sxs-lookup"><span data-stu-id="19391-163">Type</span></span>   |<span data-ttu-id="19391-164">Описание</span><span class="sxs-lookup"><span data-stu-id="19391-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19391-165">resource</span><span class="sxs-lookup"><span data-stu-id="19391-165">resource</span></span>|[<span data-ttu-id="19391-166">governanceResource</span><span class="sxs-lookup"><span data-stu-id="19391-166">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="19391-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19391-167">Read-only.</span></span> <span data-ttu-id="19391-168">Связанный ресурс для этого параметра Role.</span><span class="sxs-lookup"><span data-stu-id="19391-168">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="19391-169">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="19391-169">roleDefinition</span></span>|[<span data-ttu-id="19391-170">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="19391-170">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="19391-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19391-171">Read-only.</span></span> <span data-ttu-id="19391-172">Определение роли, принудительно заданное с помощью этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="19391-172">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19391-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19391-173">JSON representation</span></span>

<span data-ttu-id="19391-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19391-174">Here is a JSON representation of the resource.</span></span>

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
