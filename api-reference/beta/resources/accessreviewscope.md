---
title: Тип ресурса Акцессревиевскопе
description: 'В функции рецензирования Access в Azure AD — `accessReviewScope` указывает, какие сущности будут проверены при проверке доступа.  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001043"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="d1309-103">Тип ресурса Акцессревиевскопе</span><span class="sxs-lookup"><span data-stu-id="d1309-103">accessReviewScope resource type</span></span>

<span data-ttu-id="d1309-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1309-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1309-105">**Акцессревиевскопе** определяет, какие сущности будут проверены в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d1309-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="d1309-106">Он выражается в запросе OData.</span><span class="sxs-lookup"><span data-stu-id="d1309-106">This is expressed as an odata query.</span></span> <span data-ttu-id="d1309-107">Тип запроса также должен быть выражен таким образом, чтобы можно было поддерживать сценарии для просмотра сущностей за преMicrosoftGraph, таких как ARM.</span><span class="sxs-lookup"><span data-stu-id="d1309-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="d1309-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1309-108">Properties</span></span>
| <span data-ttu-id="d1309-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1309-109">Property</span></span>   | <span data-ttu-id="d1309-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1309-110">Type</span></span>  | <span data-ttu-id="d1309-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1309-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="d1309-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1309-112">query</span></span> |<span data-ttu-id="d1309-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d1309-113">String</span></span>  | <span data-ttu-id="d1309-114">Запрос, указывающий, что будет рассмотрено.</span><span class="sxs-lookup"><span data-stu-id="d1309-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="d1309-115">Примеры приведены в таблице.</span><span class="sxs-lookup"><span data-stu-id="d1309-115">See table for examples.</span></span> |
|<span data-ttu-id="d1309-116">куеритипе</span><span class="sxs-lookup"><span data-stu-id="d1309-116">queryType</span></span>  |<span data-ttu-id="d1309-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d1309-117">String</span></span> | <span data-ttu-id="d1309-118">Тип запроса.</span><span class="sxs-lookup"><span data-stu-id="d1309-118">The type of query.</span></span> <span data-ttu-id="d1309-119">Примеры включают MicrosoftGraph и ARM.</span><span class="sxs-lookup"><span data-stu-id="d1309-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="d1309-120">Поддерживаемые запросы для Акцессревиевскопе в качестве области</span><span class="sxs-lookup"><span data-stu-id="d1309-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="d1309-121">Ниже приведены запросы, поддерживаемые в качестве `scope` свойства в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d1309-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="d1309-122">Сценарий</span><span class="sxs-lookup"><span data-stu-id="d1309-122">Scenario</span></span>| <span data-ttu-id="d1309-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1309-123">Query</span></span> | <span data-ttu-id="d1309-124">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="d1309-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="d1309-125">Просмотр всех пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="d1309-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="d1309-126">Идентификатор/граупс/{грауп}/Транситивемемберс</span><span class="sxs-lookup"><span data-stu-id="d1309-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="d1309-127">Обзор гостевых пользователей, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="d1309-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="d1309-128">/граупс/{грауп ID}/Микрософт.граф.Усер/? $count = true&$filter = (userType EQ "гость")</span><span class="sxs-lookup"><span data-stu-id="d1309-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="d1309-129">Проверка пользователей, назначенных всем группам</span><span class="sxs-lookup"><span data-stu-id="d1309-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="d1309-130">./мемберс/Микрософт.граф.Усер/? $count = true&$filter = (userType EQ "гость")</span><span class="sxs-lookup"><span data-stu-id="d1309-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="d1309-131">Обратите внимание, что соответствующий Инстанцеенумератионскопе также должен быть передан в Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="d1309-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="d1309-132">В таблице ниже представлен запрос Инстанцеенумератионскопе.</span><span class="sxs-lookup"><span data-stu-id="d1309-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="d1309-133">Проверка Ассигмент на доступ к пакету управления обслуживанием</span><span class="sxs-lookup"><span data-stu-id="d1309-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="d1309-134">/Идентитиговернанце/ентитлементманажемент/акцесспаккажеассигнментс? $filter = (Акцесспаккажеид EQ "{ИД пакета}" и assignmentPolicyId EQ "{ID}")</span><span class="sxs-lookup"><span data-stu-id="d1309-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="d1309-135">Обратите внимание, что для проверки назначений пакетов Access поддерживается только чтение</span><span class="sxs-lookup"><span data-stu-id="d1309-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="d1309-136">Поддерживаемые запросы для Акцессревиевскопе как Инстанцеенумератионскопе</span><span class="sxs-lookup"><span data-stu-id="d1309-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="d1309-137">Ниже приведены запросы, поддерживаемые в качестве `instanceEnumerationScope` свойства в [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d1309-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="d1309-138">Сценарий</span><span class="sxs-lookup"><span data-stu-id="d1309-138">Scenario</span></span>| <span data-ttu-id="d1309-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1309-139">Query</span></span> | <span data-ttu-id="d1309-140">Дополнительные комментарии</span><span class="sxs-lookup"><span data-stu-id="d1309-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="d1309-141">Проверка пользователей, которым назначены все группы, за исключением указанных групп</span><span class="sxs-lookup"><span data-stu-id="d1309-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="d1309-142">/граупс? $filter = (groupTypes/Any (к:к + EQ + ' Unified ') и идентификатор Ne ' {Group ID} ' и ID Ne ' {Group ID} ' и ID Ne ' {Group ID} ') &$count = true</span><span class="sxs-lookup"><span data-stu-id="d1309-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="d1309-143">Обратите внимание, что соответствующая область также должна передаваться в Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="d1309-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="d1309-144">В разделе "Просмотр гостевых пользователей, назначенных всем группам" в таблице свойств области над запросом области.</span><span class="sxs-lookup"><span data-stu-id="d1309-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d1309-145">Связи</span><span class="sxs-lookup"><span data-stu-id="d1309-145">Relationships</span></span>
<span data-ttu-id="d1309-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1309-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1309-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d1309-147">JSON representation</span></span>
<span data-ttu-id="d1309-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1309-148">The following is a JSON representation of the resource.</span></span>
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
