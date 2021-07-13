---
title: tenantCustomizedInformation resource type
description: Представляет настраиваемые сведения для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 580479e6fd710eef7a0907ea51cd5605ef445e40
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403156"
---
# <a name="tenantcustomizedinformation-resource-type"></a><span data-ttu-id="97778-103">tenantCustomizedInformation resource type</span><span class="sxs-lookup"><span data-stu-id="97778-103">tenantCustomizedInformation resource type</span></span>

<span data-ttu-id="97778-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="97778-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97778-105">Представляет настраиваемые сведения для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="97778-105">Represents customizable information for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="97778-106">Методы</span><span class="sxs-lookup"><span data-stu-id="97778-106">Methods</span></span>
|<span data-ttu-id="97778-107">Метод</span><span class="sxs-lookup"><span data-stu-id="97778-107">Method</span></span>|<span data-ttu-id="97778-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="97778-108">Return type</span></span>|<span data-ttu-id="97778-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97778-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97778-110">Список tenantCustomizedInformations</span><span class="sxs-lookup"><span data-stu-id="97778-110">List tenantCustomizedInformations</span></span>](../api/managedtenants-managedtenant-list-tenantscustomizedinformation.md)|<span data-ttu-id="97778-111">[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection</span><span class="sxs-lookup"><span data-stu-id="97778-111">[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection</span></span>|<span data-ttu-id="97778-112">Получите список объектов [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="97778-112">Get a list of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) objects and their properties.</span></span>|
|[<span data-ttu-id="97778-113">Get tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="97778-113">Get tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-get.md)|[<span data-ttu-id="97778-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="97778-114">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="97778-115">Ознакомьтесь с свойствами и отношениями объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="97778-115">Read the properties and relationships of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|
|[<span data-ttu-id="97778-116">Обновление tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="97778-116">Update tenantCustomizedInformation</span></span>](../api/managedtenants-tenantcustomizedinformation-update.md)|[<span data-ttu-id="97778-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="97778-117">microsoft.graph.managedTenants.tenantCustomizedInformation</span></span>](../resources/managedtenants-tenantcustomizedinformation.md)|<span data-ttu-id="97778-118">Обновление свойств объекта [tenantCustomizedInformation.](../resources/managedtenants-tenantcustomizedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="97778-118">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="97778-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="97778-119">Properties</span></span>
|<span data-ttu-id="97778-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="97778-120">Property</span></span>|<span data-ttu-id="97778-121">Тип</span><span class="sxs-lookup"><span data-stu-id="97778-121">Type</span></span>|<span data-ttu-id="97778-122">Описание</span><span class="sxs-lookup"><span data-stu-id="97778-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97778-123">contacts</span><span class="sxs-lookup"><span data-stu-id="97778-123">contacts</span></span>|<span data-ttu-id="97778-124">[коллекция microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md)</span><span class="sxs-lookup"><span data-stu-id="97778-124">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="97778-125">Коллекция контактов для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="97778-125">The collection of contacts for the managed tenant.</span></span> <span data-ttu-id="97778-126">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="97778-126">Optional.</span></span>|
|<span data-ttu-id="97778-127">displayName</span><span class="sxs-lookup"><span data-stu-id="97778-127">displayName</span></span>|<span data-ttu-id="97778-128">String</span><span class="sxs-lookup"><span data-stu-id="97778-128">String</span></span>|<span data-ttu-id="97778-129">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="97778-129">The display name for the managed tenant.</span></span> <span data-ttu-id="97778-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97778-130">Required.</span></span> <span data-ttu-id="97778-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97778-131">Read-only.</span></span>|
|<span data-ttu-id="97778-132">id</span><span class="sxs-lookup"><span data-stu-id="97778-132">id</span></span>|<span data-ttu-id="97778-133">String</span><span class="sxs-lookup"><span data-stu-id="97778-133">String</span></span>|<span data-ttu-id="97778-134">Идентификатор Azure Active Directory клиента для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="97778-134">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="97778-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97778-135">Required.</span></span> <span data-ttu-id="97778-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97778-136">Read-only.</span></span>|
|<span data-ttu-id="97778-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="97778-137">tenantId</span></span>|<span data-ttu-id="97778-138">String</span><span class="sxs-lookup"><span data-stu-id="97778-138">String</span></span>|<span data-ttu-id="97778-139">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="97778-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="97778-140">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="97778-140">Optional.</span></span> <span data-ttu-id="97778-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97778-141">Read-only.</span></span>|
|<span data-ttu-id="97778-142">веб-сайт</span><span class="sxs-lookup"><span data-stu-id="97778-142">website</span></span>|<span data-ttu-id="97778-143">String</span><span class="sxs-lookup"><span data-stu-id="97778-143">String</span></span>|<span data-ttu-id="97778-144">Веб-сайт управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="97778-144">The website for the managed tenant.</span></span> <span data-ttu-id="97778-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97778-145">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97778-146">Связи</span><span class="sxs-lookup"><span data-stu-id="97778-146">Relationships</span></span>
<span data-ttu-id="97778-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97778-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97778-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97778-148">JSON representation</span></span>
<span data-ttu-id="97778-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97778-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```
