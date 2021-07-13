---
title: тип ресурса tenantStatusInformation
description: Представляет сведения о состоянии на борту для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3e01ac003cda223788e0fc8e6dae01f18667da11
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402687"
---
# <a name="tenantstatusinformation-resource-type"></a><span data-ttu-id="14982-103">тип ресурса tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="14982-103">tenantStatusInformation resource type</span></span>

<span data-ttu-id="14982-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="14982-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14982-105">Представляет сведения о состоянии на борту для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="14982-105">Represents onboarding status information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="14982-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="14982-106">Properties</span></span>
|<span data-ttu-id="14982-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="14982-107">Property</span></span>|<span data-ttu-id="14982-108">Тип</span><span class="sxs-lookup"><span data-stu-id="14982-108">Type</span></span>|<span data-ttu-id="14982-109">Описание</span><span class="sxs-lookup"><span data-stu-id="14982-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14982-110">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="14982-110">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="14982-111">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="14982-111">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="14982-112">Состояние отношения привилегий делегирования администратора между управляющей организацией и управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="14982-112">The status of the delegated admin privilege relationship between the managing entity and the managed tenant.</span></span> <span data-ttu-id="14982-113">Возможные значения: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="14982-113">Possible values are: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`.</span></span> <span data-ttu-id="14982-114">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-114">Optional.</span></span> <span data-ttu-id="14982-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-115">Read-only.</span></span>|
|<span data-ttu-id="14982-116">lastDelegatedPrivilegeRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="14982-116">lastDelegatedPrivilegeRefreshDateTime</span></span>|<span data-ttu-id="14982-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14982-117">DateTimeOffset</span></span>|<span data-ttu-id="14982-118">Дата и время обновления статуса делегирования привилегий администратора.</span><span class="sxs-lookup"><span data-stu-id="14982-118">The date and time the delegated admin privileges status was updated.</span></span> <span data-ttu-id="14982-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-119">Optional.</span></span> <span data-ttu-id="14982-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-120">Read-only.</span></span>|
|<span data-ttu-id="14982-121">offboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="14982-121">offboardedByUserId</span></span>|<span data-ttu-id="14982-122">String</span><span class="sxs-lookup"><span data-stu-id="14982-122">String</span></span>|<span data-ttu-id="14982-123">Идентификатор учетной записи, которая отключалась от управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="14982-123">The identifier for the account that offboarded the managed tenant.</span></span> <span data-ttu-id="14982-124">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-124">Optional.</span></span> <span data-ttu-id="14982-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-125">Read-only.</span></span>|
|<span data-ttu-id="14982-126">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="14982-126">offboardedDateTime</span></span>|<span data-ttu-id="14982-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14982-127">DateTimeOffset</span></span>|<span data-ttu-id="14982-128">Дата и время отключения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="14982-128">The date and time when the managed tenant was offboarded.</span></span> <span data-ttu-id="14982-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-129">Optional.</span></span> <span data-ttu-id="14982-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-130">Read-only.</span></span>|
|<span data-ttu-id="14982-131">onboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="14982-131">onboardedByUserId</span></span>|<span data-ttu-id="14982-132">String</span><span class="sxs-lookup"><span data-stu-id="14982-132">String</span></span>|<span data-ttu-id="14982-133">Идентификатор учетной записи, в которую вошел управляемый клиент.</span><span class="sxs-lookup"><span data-stu-id="14982-133">The identifier for the account that onboarded the managed tenant.</span></span> <span data-ttu-id="14982-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-134">Optional.</span></span> <span data-ttu-id="14982-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-135">Read-only.</span></span>|
|<span data-ttu-id="14982-136">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="14982-136">onboardedDateTime</span></span>|<span data-ttu-id="14982-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14982-137">DateTimeOffset</span></span>|<span data-ttu-id="14982-138">Дата и время, когда управляемый клиент был на борту.</span><span class="sxs-lookup"><span data-stu-id="14982-138">The date and time when the managed tenant was onboarded.</span></span> <span data-ttu-id="14982-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-139">Optional.</span></span> <span data-ttu-id="14982-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-140">Read-only.</span></span>|
|<span data-ttu-id="14982-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="14982-141">onboardingStatus</span></span>|<span data-ttu-id="14982-142">tenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="14982-142">tenantOnboardingStatus</span></span>|<span data-ttu-id="14982-143">Состояние onboarding для управляемого клиента..</span><span class="sxs-lookup"><span data-stu-id="14982-143">The onboarding status for the managed tenant..</span></span> <span data-ttu-id="14982-144">Возможные значения: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="14982-144">Possible values are: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`.</span></span> <span data-ttu-id="14982-145">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-145">Optional.</span></span> <span data-ttu-id="14982-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-146">Read-only.</span></span>|
|<span data-ttu-id="14982-147">workloadStatuses</span><span class="sxs-lookup"><span data-stu-id="14982-147">workloadStatuses</span></span>|<span data-ttu-id="14982-148">[коллекция microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md)</span><span class="sxs-lookup"><span data-stu-id="14982-148">[microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md) collection</span></span>|<span data-ttu-id="14982-149">Коллекция статуй рабочей нагрузки для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="14982-149">The collection of workload statues for the managed tenant.</span></span> <span data-ttu-id="14982-150">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="14982-150">Optional.</span></span> <span data-ttu-id="14982-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14982-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14982-152">Связи</span><span class="sxs-lookup"><span data-stu-id="14982-152">Relationships</span></span>
<span data-ttu-id="14982-153">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14982-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14982-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14982-154">JSON representation</span></span>
<span data-ttu-id="14982-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14982-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
