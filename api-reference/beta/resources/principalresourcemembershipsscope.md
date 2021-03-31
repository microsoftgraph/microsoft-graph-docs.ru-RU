---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет для областей выбора просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2ac3dd53223b9260c3f51c3c872d36b044e698d5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469790"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="576c1-103">тип ресурса principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="576c1-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="576c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="576c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="576c1-105">PrincipalResourceMembershipsScope — это тип [accessReviewScope,](accessreviewscope.md) который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и просмотреть доступ выбранных директоров к выбранным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="576c1-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="576c1-106">См. поддерживаемые запросы, чтобы узнать, что можно выбрать.</span><span class="sxs-lookup"><span data-stu-id="576c1-106">See the supported queries to see what can be selected.</span></span> <span data-ttu-id="576c1-107">Он используется в качестве `scope` свойства [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="576c1-107">It is used as the `scope` property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="576c1-108">Наследует [от accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="576c1-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="576c1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="576c1-109">Properties</span></span>
|<span data-ttu-id="576c1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="576c1-110">Property</span></span>|<span data-ttu-id="576c1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="576c1-111">Type</span></span>|<span data-ttu-id="576c1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="576c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="576c1-113">principalScopes</span><span class="sxs-lookup"><span data-stu-id="576c1-113">principalScopes</span></span>|<span data-ttu-id="576c1-114">[коллекция accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="576c1-114">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="576c1-115">Определяет области, включаемые в обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="576c1-115">Defines the scopes of the principals to be included in an access review.</span></span>|
|<span data-ttu-id="576c1-116">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="576c1-116">resourceScopes</span></span>|<span data-ttu-id="576c1-117">[коллекция accessReviewScope](../resources/accessreviewscope.md)</span><span class="sxs-lookup"><span data-stu-id="576c1-117">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="576c1-118">Определяет области ресурсов, для которых будет рассмотрен доступ.</span><span class="sxs-lookup"><span data-stu-id="576c1-118">Defines the scopes of the resources for which access will be reviewed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="576c1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="576c1-119">Relationships</span></span>
<span data-ttu-id="576c1-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="576c1-120">None.</span></span>

### <a name="supported-queries-for-resourcescope"></a><span data-ttu-id="576c1-121">Поддерживаемые запросы для resourceScope</span><span class="sxs-lookup"><span data-stu-id="576c1-121">Supported queries for resourceScope</span></span>
<span data-ttu-id="576c1-122">Запросы поддерживаются как `resourceScope` свойство.</span><span class="sxs-lookup"><span data-stu-id="576c1-122">The queries are supported as the `resourceScope` property.</span></span> <span data-ttu-id="576c1-123">Они определяют, к каков набор доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="576c1-123">They determine the set of resources access is being reviewed to.</span></span> 

|<span data-ttu-id="576c1-124">Сценарий</span><span class="sxs-lookup"><span data-stu-id="576c1-124">Scenario</span></span>| <span data-ttu-id="576c1-125">запрос resourceScope</span><span class="sxs-lookup"><span data-stu-id="576c1-125">resourceScope Query</span></span> | 
|--|--|
| <span data-ttu-id="576c1-126">Проверка доступа principalScopes к основной службе</span><span class="sxs-lookup"><span data-stu-id="576c1-126">Reviewing access of principalScopes to a service principal</span></span> | <span data-ttu-id="576c1-127">/servicePrincipals/{service principal ID}</span><span class="sxs-lookup"><span data-stu-id="576c1-127">/servicePrincipals/{service principal ID}</span></span> |
| <span data-ttu-id="576c1-128">Просмотр доступа principalScopes к роли каталога Azure AD</span><span class="sxs-lookup"><span data-stu-id="576c1-128">Reviewing access of principalScopes to an Azure AD directory role</span></span> | <span data-ttu-id="576c1-129">/roleManagement/directory/roleDefinitions/{role ID}</span><span class="sxs-lookup"><span data-stu-id="576c1-129">/roleManagement/directory/roleDefinitions/{role ID}</span></span> |
| <span data-ttu-id="576c1-130">Просмотр доступа principalScopes ко всем ролям каталога Azure AD</span><span class="sxs-lookup"><span data-stu-id="576c1-130">Reviewing access of principalScopes to all Azure AD directory roles</span></span> | <span data-ttu-id="576c1-131">/roleManagement/directory/roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="576c1-131">/roleManagement/directory/roleDefinitions</span></span> |

### <a name="supported-queries-for-principalscope"></a><span data-ttu-id="576c1-132">Поддерживаемые запросы для principalScope</span><span class="sxs-lookup"><span data-stu-id="576c1-132">Supported queries for principalScope</span></span>
<span data-ttu-id="576c1-133">Запросы поддерживаются как `principalScope` свойство.</span><span class="sxs-lookup"><span data-stu-id="576c1-133">The queries are supported as the `principalScope` property.</span></span> <span data-ttu-id="576c1-134">Они определяют набор директоров, доступ которых к связанному ресурсуScope будет рассмотрен.</span><span class="sxs-lookup"><span data-stu-id="576c1-134">They determine the set of principals whose access to the associated resourceScope will be reviewed.</span></span> <span data-ttu-id="576c1-135">В связанном типе principalScope перечислены типы запросов odata, принятые в качестве principalScope.</span><span class="sxs-lookup"><span data-stu-id="576c1-135">The associated principalScope Type lists the odata query types accepted as the principalScope.</span></span>

|<span data-ttu-id="576c1-136">Сценарий</span><span class="sxs-lookup"><span data-stu-id="576c1-136">Scenario</span></span>| <span data-ttu-id="576c1-137">запрос principalScope</span><span class="sxs-lookup"><span data-stu-id="576c1-137">principalScope Query</span></span> | <span data-ttu-id="576c1-138">Тип запроса OData</span><span class="sxs-lookup"><span data-stu-id="576c1-138">OData Query Type</span></span> | <span data-ttu-id="576c1-139">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="576c1-139">Additional Comments</span></span> |
|--|--|-- | --|
| <span data-ttu-id="576c1-140">Просмотр доступа всех пользователей к ресурсуScope</span><span class="sxs-lookup"><span data-stu-id="576c1-140">Review access of all users to the resourceScope</span></span> | <span data-ttu-id="576c1-141">/users</span><span class="sxs-lookup"><span data-stu-id="576c1-141">/users</span></span> |[<span data-ttu-id="576c1-142">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="576c1-142">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="576c1-143">Просмотр доступа гостевых пользователей к ресурсуScope</span><span class="sxs-lookup"><span data-stu-id="576c1-143">Review access of  guest users to the resourceScope</span></span> | <span data-ttu-id="576c1-144">/users?$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="576c1-144">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="576c1-145">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="576c1-145">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="576c1-146">Просмотр доступа всех неактивных пользователей к ресурсуScope</span><span class="sxs-lookup"><span data-stu-id="576c1-146">Review access of all inactive users to the resourceScope</span></span> | <span data-ttu-id="576c1-147">/users</span><span class="sxs-lookup"><span data-stu-id="576c1-147">/users</span></span> |[<span data-ttu-id="576c1-148">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="576c1-148">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="576c1-149">Должно включать `instanceDuration` свойство</span><span class="sxs-lookup"><span data-stu-id="576c1-149">Must include `instanceDuration` property</span></span>|
| <span data-ttu-id="576c1-150">Просмотр доступа неактивных пользователей гостей к ресурсуScope</span><span class="sxs-lookup"><span data-stu-id="576c1-150">Review access of guest inactive users to the resourceScope</span></span> | <span data-ttu-id="576c1-151">/users?$filter=(userType eq 'Guest')</span><span class="sxs-lookup"><span data-stu-id="576c1-151">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="576c1-152">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="576c1-152">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="576c1-153">Должно включать `instanceDuration` свойство</span><span class="sxs-lookup"><span data-stu-id="576c1-153">Must include `instanceDuration` property</span></span>|




## <a name="json-representation"></a><span data-ttu-id="576c1-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="576c1-154">JSON representation</span></span>
<span data-ttu-id="576c1-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="576c1-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
