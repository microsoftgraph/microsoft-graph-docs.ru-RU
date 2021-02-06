---
title: Тип ресурса accessReviewScope
description: 'В функции проверки доступа Azure AD объекты, которые будут рассмотрены в `accessReviewScope` проверке доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133447"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="542dd-103">Тип ресурса accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="542dd-103">accessReviewScope resource type</span></span>

<span data-ttu-id="542dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="542dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="542dd-105">**AccessReviewScope** определяет, какие сущности будут рассмотрены в [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="542dd-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="542dd-106">Это выражается как запрос odata.</span><span class="sxs-lookup"><span data-stu-id="542dd-106">This is expressed as an odata query.</span></span> <span data-ttu-id="542dd-107">Тип запроса также должен быть выражен, чтобы сценарии можно было поддерживать для просмотра сущностями за пределами MicrosoftGraph, например ARM.</span><span class="sxs-lookup"><span data-stu-id="542dd-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="542dd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="542dd-108">Properties</span></span>
| <span data-ttu-id="542dd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="542dd-109">Property</span></span>   | <span data-ttu-id="542dd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="542dd-110">Type</span></span>  | <span data-ttu-id="542dd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="542dd-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="542dd-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="542dd-112">query</span></span> |<span data-ttu-id="542dd-113">Строка</span><span class="sxs-lookup"><span data-stu-id="542dd-113">String</span></span>  | <span data-ttu-id="542dd-114">Запрос, определяющий, что будет рассмотрено.</span><span class="sxs-lookup"><span data-stu-id="542dd-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="542dd-115">Примеры см. в таблице.</span><span class="sxs-lookup"><span data-stu-id="542dd-115">See table for examples.</span></span> |
|<span data-ttu-id="542dd-116">queryType</span><span class="sxs-lookup"><span data-stu-id="542dd-116">queryType</span></span>  |<span data-ttu-id="542dd-117">Строка</span><span class="sxs-lookup"><span data-stu-id="542dd-117">String</span></span> | <span data-ttu-id="542dd-118">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="542dd-118">The type of query.</span></span> <span data-ttu-id="542dd-119">Примеры: MicrosoftGraph и ARM.</span><span class="sxs-lookup"><span data-stu-id="542dd-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="542dd-120">Поддерживаемые запросы для accessReviewScope в качестве области</span><span class="sxs-lookup"><span data-stu-id="542dd-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="542dd-121">Далее запросы поддерживаются в качестве `scope` свойства [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="542dd-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="542dd-122">Сценарий</span><span class="sxs-lookup"><span data-stu-id="542dd-122">Scenario</span></span>| <span data-ttu-id="542dd-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="542dd-123">Query</span></span> | <span data-ttu-id="542dd-124">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="542dd-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="542dd-125">Проверка всех пользователей, которые назначены группе</span><span class="sxs-lookup"><span data-stu-id="542dd-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="542dd-126">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="542dd-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="542dd-127">Просмотр гостевых пользователей, присвоенных группе</span><span class="sxs-lookup"><span data-stu-id="542dd-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="542dd-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="542dd-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="542dd-129">Проверка гостевых пользователей, присвоенных всем группам</span><span class="sxs-lookup"><span data-stu-id="542dd-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="542dd-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="542dd-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="542dd-131">Обратите внимание, что соответствующий экземплярEnumerationScope также следует передать в accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="542dd-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="542dd-132">См. таблицу ниже для запроса instanceEnumerationScope.</span><span class="sxs-lookup"><span data-stu-id="542dd-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="542dd-133">Проверки пакета управления правами на доступ к данным</span><span class="sxs-lookup"><span data-stu-id="542dd-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="542dd-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span><span class="sxs-lookup"><span data-stu-id="542dd-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="542dd-135">Обратите внимание, что для проверки назначения пакета Access поддерживается только чтение</span><span class="sxs-lookup"><span data-stu-id="542dd-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="542dd-136">Поддерживаемые запросы для accessReviewScope как instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="542dd-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="542dd-137">Далее запросы поддерживаются в качестве `instanceEnumerationScope` свойства [в accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="542dd-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="542dd-138">Сценарий</span><span class="sxs-lookup"><span data-stu-id="542dd-138">Scenario</span></span>| <span data-ttu-id="542dd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="542dd-139">Query</span></span> | <span data-ttu-id="542dd-140">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="542dd-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="542dd-141">Просмотр гостевых пользователей, которые назначены всем группам, за исключением указанных групп</span><span class="sxs-lookup"><span data-stu-id="542dd-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="542dd-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span><span class="sxs-lookup"><span data-stu-id="542dd-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="542dd-143">Обратите внимание, что соответствующая область также должна быть передана в accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="542dd-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="542dd-144">См. выше в таблице свойств области "Просмотр гостевых пользователей, присвоенных всем группам" запроса области.</span><span class="sxs-lookup"><span data-stu-id="542dd-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="542dd-145">Связи</span><span class="sxs-lookup"><span data-stu-id="542dd-145">Relationships</span></span>
<span data-ttu-id="542dd-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="542dd-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="542dd-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="542dd-147">JSON representation</span></span>
<span data-ttu-id="542dd-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="542dd-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
