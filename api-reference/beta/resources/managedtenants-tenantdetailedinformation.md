---
title: тип ресурса tenantDetailedInformation
description: Представляет подробные сведения для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 40aa157b12ccef64b6eb7ab6c92349a3e74745f8
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402694"
---
# <a name="tenantdetailedinformation-resource-type"></a><span data-ttu-id="9ac0e-103">тип ресурса tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="9ac0e-103">tenantDetailedInformation resource type</span></span>

<span data-ttu-id="9ac0e-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9ac0e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac0e-105">Представляет подробные сведения для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-105">Represents detailed information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="9ac0e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9ac0e-106">Methods</span></span>
|<span data-ttu-id="9ac0e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9ac0e-107">Method</span></span>|<span data-ttu-id="9ac0e-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9ac0e-108">Return type</span></span>|<span data-ttu-id="9ac0e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac0e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ac0e-110">Список tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="9ac0e-110">List tenantDetailedInformation</span></span>](../api/managedtenants-managedtenant-list-tenantsdetailedinformation.md)|<span data-ttu-id="9ac0e-111">[коллекция microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="9ac0e-111">[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) collection</span></span>|<span data-ttu-id="9ac0e-112">Получите список объектов [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-112">Get a list of the [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="9ac0e-113">Get tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="9ac0e-113">Get tenantDetailedInformation</span></span>](../api/managedtenants-tenantdetailedinformation-get.md)|[<span data-ttu-id="9ac0e-114">microsoft.graph.managedTenants.tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="9ac0e-114">microsoft.graph.managedTenants.tenantDetailedInformation</span></span>](../resources/managedtenants-tenantdetailedinformation.md)|<span data-ttu-id="9ac0e-115">Ознакомьтесь с свойствами и отношениями объекта [tenantDetailedInformation.](../resources/managedtenants-tenantdetailedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="9ac0e-115">Read the properties and relationships of a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ac0e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ac0e-116">Properties</span></span>
|<span data-ttu-id="9ac0e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ac0e-117">Property</span></span>|<span data-ttu-id="9ac0e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9ac0e-118">Type</span></span>|<span data-ttu-id="9ac0e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac0e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac0e-120">city</span><span class="sxs-lookup"><span data-stu-id="9ac0e-120">city</span></span>|<span data-ttu-id="9ac0e-121">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-121">String</span></span>|<span data-ttu-id="9ac0e-122">Город, в котором расположен управляемый клиент.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-122">The city where the managed tenant is located.</span></span> <span data-ttu-id="9ac0e-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-123">Optional.</span></span> <span data-ttu-id="9ac0e-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-124">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-125">countryCode</span><span class="sxs-lookup"><span data-stu-id="9ac0e-125">countryCode</span></span>|<span data-ttu-id="9ac0e-126">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-126">String</span></span>|<span data-ttu-id="9ac0e-127">Код для страны, в которой расположен управляемый клиент.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-127">The code for the country where the managed tenant is located.</span></span> <span data-ttu-id="9ac0e-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-128">Optional.</span></span> <span data-ttu-id="9ac0e-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-129">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-130">countryName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-130">countryName</span></span>|<span data-ttu-id="9ac0e-131">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-131">String</span></span>|<span data-ttu-id="9ac0e-132">Имя страны, в которой расположен управляемый клиент.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-132">The name for the country where the managed tenant is located.</span></span> <span data-ttu-id="9ac0e-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-133">Optional.</span></span> <span data-ttu-id="9ac0e-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-134">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-135">defaultDomainName</span></span>|<span data-ttu-id="9ac0e-136">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-136">String</span></span>|<span data-ttu-id="9ac0e-137">Доменное имя по умолчанию для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-137">The default domain name for the managed tenant.</span></span> <span data-ttu-id="9ac0e-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-138">Optional.</span></span> <span data-ttu-id="9ac0e-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-139">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-140">displayName</span></span>|<span data-ttu-id="9ac0e-141">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-141">String</span></span>|<span data-ttu-id="9ac0e-142">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-142">The display name for the managed tenant.</span></span>|
|<span data-ttu-id="9ac0e-143">id</span><span class="sxs-lookup"><span data-stu-id="9ac0e-143">id</span></span>|<span data-ttu-id="9ac0e-144">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-144">String</span></span>|<span data-ttu-id="9ac0e-145">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-145">The unique identifier for this entity.</span></span> <span data-ttu-id="9ac0e-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-146">Required.</span></span> <span data-ttu-id="9ac0e-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-147">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-148">industryName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-148">industryName</span></span>|<span data-ttu-id="9ac0e-149">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-149">String</span></span>|<span data-ttu-id="9ac0e-150">Бизнес-индустрия, связанная с управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-150">The business industry associated with the managed tenant.</span></span> <span data-ttu-id="9ac0e-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-151">Optional.</span></span> <span data-ttu-id="9ac0e-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-152">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-153">регион</span><span class="sxs-lookup"><span data-stu-id="9ac0e-153">region</span></span>|<span data-ttu-id="9ac0e-154">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-154">String</span></span>|<span data-ttu-id="9ac0e-155">Регион, в котором расположен управляемый клиент.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-155">The region where the managed tenant is located.</span></span> <span data-ttu-id="9ac0e-156">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-156">Optional.</span></span> <span data-ttu-id="9ac0e-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-157">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-158">segmentName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-158">segmentName</span></span>|<span data-ttu-id="9ac0e-159">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-159">String</span></span>|<span data-ttu-id="9ac0e-160">Бизнес-сегмент, связанный с управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-160">The business segment associated with the managed tenant.</span></span> <span data-ttu-id="9ac0e-161">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-161">Optional.</span></span> <span data-ttu-id="9ac0e-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-162">Read-only.</span></span>|
|<span data-ttu-id="9ac0e-163">tenantId</span><span class="sxs-lookup"><span data-stu-id="9ac0e-163">tenantId</span></span>|<span data-ttu-id="9ac0e-164">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-164">String</span></span>|<span data-ttu-id="9ac0e-165">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="9ac0e-165">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="9ac0e-166">verticalName</span><span class="sxs-lookup"><span data-stu-id="9ac0e-166">verticalName</span></span>|<span data-ttu-id="9ac0e-167">String</span><span class="sxs-lookup"><span data-stu-id="9ac0e-167">String</span></span>|<span data-ttu-id="9ac0e-168">Вертикаль, связанная с управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-168">The vertical associated with the managed tenant.</span></span> <span data-ttu-id="9ac0e-169">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-169">Optional.</span></span> <span data-ttu-id="9ac0e-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac0e-171">Связи</span><span class="sxs-lookup"><span data-stu-id="9ac0e-171">Relationships</span></span>
<span data-ttu-id="9ac0e-172">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ac0e-173">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ac0e-173">JSON representation</span></span>
<span data-ttu-id="9ac0e-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ac0e-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "defaultDomainName": "String",
  "countryName": "String",
  "countryCode": "String",
  "city": "String",
  "region": "String",
  "verticalName": "String",
  "industryName": "String",
  "segmentName": "String"
}
```

