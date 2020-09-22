---
title: Тип ресурса Говернанцеролесеттинг
description: Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 61889ef9f5ecd968b52704138260d3b39ceaf961
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081645"
---
# <a name="governancerolesetting-resource-type"></a><span data-ttu-id="304c2-103">Тип ресурса Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="304c2-103">governanceRoleSetting resource type</span></span>

<span data-ttu-id="304c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304c2-105">Представляет набор конфигураций для каждого определения роли, которые необходимо оценить при создании или изменении назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="304c2-105">Represents a set of configurations on each role definition that needs to be evaluated against when role assignments are created or modified.</span></span> <span data-ttu-id="304c2-106">Например, параметры роли могут включать правило "максимальная длительность назначения", правило "MFA Required on Activation" и т. д.</span><span class="sxs-lookup"><span data-stu-id="304c2-106">For example, role settings might include "maximum assignment duration" rule, "MFA required on activation" rule, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="304c2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="304c2-107">Methods</span></span>

| <span data-ttu-id="304c2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="304c2-108">Method</span></span>          | <span data-ttu-id="304c2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="304c2-109">Return Type</span></span> |<span data-ttu-id="304c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="304c2-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="304c2-111">Перечисление</span><span class="sxs-lookup"><span data-stu-id="304c2-111">List</span></span>](../api/governancerolesetting-list.md) | <span data-ttu-id="304c2-112">Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="304c2-112">[governanceRoleSetting](../resources/governancerolesetting.md) collection</span></span>|<span data-ttu-id="304c2-113">Перечисление коллекции параметров роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="304c2-113">List a collection of role settings on a resource.</span></span>|
|[<span data-ttu-id="304c2-114">Получение</span><span class="sxs-lookup"><span data-stu-id="304c2-114">Get</span></span>](../api/governancerolesetting-get.md) |  [<span data-ttu-id="304c2-115">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="304c2-115">governanceRoleSetting</span></span>](../resources/governancerolesetting.md) |<span data-ttu-id="304c2-116">Чтение свойств и связей параметра Role.</span><span class="sxs-lookup"><span data-stu-id="304c2-116">Read properties and relationships of a role setting.</span></span>|
|[<span data-ttu-id="304c2-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="304c2-117">Update</span></span>](../api/governancerolesetting-update.md) | [<span data-ttu-id="304c2-118">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="304c2-118">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)  |<span data-ttu-id="304c2-119">Обновление объекта параметров роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-119">Update a role setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="304c2-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="304c2-120">Properties</span></span>
|<span data-ttu-id="304c2-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="304c2-121">Property</span></span>               |<span data-ttu-id="304c2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="304c2-122">Type</span></span>                                      |<span data-ttu-id="304c2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="304c2-123">Description</span></span>|
|:--------------------|:---------------------------------------|:----------|
|<span data-ttu-id="304c2-124">id</span><span class="sxs-lookup"><span data-stu-id="304c2-124">id</span></span>                   |<span data-ttu-id="304c2-125">Строка</span><span class="sxs-lookup"><span data-stu-id="304c2-125">String</span></span>                                  |<span data-ttu-id="304c2-126">Идентификатор Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="304c2-126">The id of the roleSetting.</span></span>|
|<span data-ttu-id="304c2-127">resourceId</span><span class="sxs-lookup"><span data-stu-id="304c2-127">resourceId</span></span>           |<span data-ttu-id="304c2-128">String</span><span class="sxs-lookup"><span data-stu-id="304c2-128">String</span></span>                                  |<span data-ttu-id="304c2-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="304c2-129">Required.</span></span> <span data-ttu-id="304c2-130">Идентификатор ресурса, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-130">The id of the resource that the role setting is associated with.</span></span>|
|<span data-ttu-id="304c2-131">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="304c2-131">roleDefinitionId</span></span>     |<span data-ttu-id="304c2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="304c2-132">String</span></span>                                  |<span data-ttu-id="304c2-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="304c2-133">Required.</span></span> <span data-ttu-id="304c2-134">Идентификатор определения роли, с которым связана Настройка роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-134">The id of the role definition that the role setting is associated with.</span></span>|
|<span data-ttu-id="304c2-135">isDefault</span><span class="sxs-lookup"><span data-stu-id="304c2-135">isDefault</span></span>            |<span data-ttu-id="304c2-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="304c2-136">Boolean</span></span>                                 |<span data-ttu-id="304c2-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="304c2-137">Read-only.</span></span> <span data-ttu-id="304c2-138">Указывает, является ли Ролесеттинг Ролесеттинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="304c2-138">Indicate if the roleSetting is a default roleSetting</span></span>|
|<span data-ttu-id="304c2-139">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="304c2-139">lastUpdatedDateTime</span></span>  |<span data-ttu-id="304c2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="304c2-140">DateTimeOffset</span></span>                          |<span data-ttu-id="304c2-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="304c2-141">Read-only.</span></span> <span data-ttu-id="304c2-142">Время последнего обновления параметра роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-142">The time when the role setting was last updated.</span></span> <span data-ttu-id="304c2-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="304c2-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="304c2-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="304c2-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="304c2-145">ластупдатедби</span><span class="sxs-lookup"><span data-stu-id="304c2-145">lastUpdatedBy</span></span>        |<span data-ttu-id="304c2-146">String</span><span class="sxs-lookup"><span data-stu-id="304c2-146">String</span></span>                                  |<span data-ttu-id="304c2-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="304c2-147">Read-only.</span></span> <span data-ttu-id="304c2-148">Отображаемое имя администратора, который последним обновил Ролесеттинг.</span><span class="sxs-lookup"><span data-stu-id="304c2-148">The display name of the administrator who last updated the roleSetting.</span></span>|
|<span data-ttu-id="304c2-149">админелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="304c2-149">adminEligibleSettings</span></span>|<span data-ttu-id="304c2-150">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="304c2-150">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="304c2-151">Параметры правил, которые оцениваются, когда администратор пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-151">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="304c2-152">админмемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="304c2-152">adminMemberSettings</span></span>  |<span data-ttu-id="304c2-153">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="304c2-153">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="304c2-154">Параметры правил, которые оцениваются при попытке администратора добавить назначение роли прямого члена.</span><span class="sxs-lookup"><span data-stu-id="304c2-154">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="304c2-155">усерелигиблесеттингс</span><span class="sxs-lookup"><span data-stu-id="304c2-155">userEligibleSettings</span></span> |<span data-ttu-id="304c2-156">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="304c2-156">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="304c2-157">Параметры правил, которые оцениваются, когда пользователь пытается добавить подходящего назначения роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-157">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="304c2-158">Этот параметр не поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="304c2-158">The setting is not supported for now.</span></span>|
|<span data-ttu-id="304c2-159">усермемберсеттингс</span><span class="sxs-lookup"><span data-stu-id="304c2-159">userMemberSettings</span></span>   |<span data-ttu-id="304c2-160">Коллекция [говернанцерулесеттинг](../resources/governancerulesetting.md)</span><span class="sxs-lookup"><span data-stu-id="304c2-160">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="304c2-161">Параметры правил, которые оцениваются, когда пользователь пытается активировать назначение роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-161">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="304c2-162">Связи</span><span class="sxs-lookup"><span data-stu-id="304c2-162">Relationships</span></span>
| <span data-ttu-id="304c2-163">Связь</span><span class="sxs-lookup"><span data-stu-id="304c2-163">Relationship</span></span> | <span data-ttu-id="304c2-164">Тип</span><span class="sxs-lookup"><span data-stu-id="304c2-164">Type</span></span>   |<span data-ttu-id="304c2-165">Описание</span><span class="sxs-lookup"><span data-stu-id="304c2-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="304c2-166">resource</span><span class="sxs-lookup"><span data-stu-id="304c2-166">resource</span></span>|[<span data-ttu-id="304c2-167">governanceResource</span><span class="sxs-lookup"><span data-stu-id="304c2-167">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="304c2-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="304c2-168">Read-only.</span></span> <span data-ttu-id="304c2-169">Связанный ресурс для этого параметра Role.</span><span class="sxs-lookup"><span data-stu-id="304c2-169">The associated resource for this role setting.</span></span>|
|<span data-ttu-id="304c2-170">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="304c2-170">roleDefinition</span></span>|[<span data-ttu-id="304c2-171">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="304c2-171">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md)|<span data-ttu-id="304c2-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="304c2-172">Read-only.</span></span> <span data-ttu-id="304c2-173">Определение роли, принудительно заданное с помощью этого параметра роли.</span><span class="sxs-lookup"><span data-stu-id="304c2-173">The role definition that is enforced with this role setting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="304c2-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="304c2-174">JSON representation</span></span>

<span data-ttu-id="304c2-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="304c2-175">Here is a JSON representation of the resource.</span></span>

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


