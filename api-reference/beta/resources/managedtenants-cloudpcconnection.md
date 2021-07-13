---
title: тип ресурса cloudPcConnection
description: Представляет облачное подключение к ПК для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 75af7be7633e43bc594f7185f196f40abca39883
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402550"
---
# <a name="cloudpcconnection-resource-type"></a><span data-ttu-id="4489e-103">тип ресурса cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="4489e-103">cloudPcConnection resource type</span></span>

<span data-ttu-id="4489e-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="4489e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4489e-105">Представляет облачное подключение к ПК для данного управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="4489e-105">Represents a cloud PC connection for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="4489e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4489e-106">Methods</span></span>
|<span data-ttu-id="4489e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4489e-107">Method</span></span>|<span data-ttu-id="4489e-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4489e-108">Return type</span></span>|<span data-ttu-id="4489e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4489e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4489e-110">Список cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="4489e-110">List cloudPcConnections</span></span>](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|<span data-ttu-id="4489e-111">[коллекция microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="4489e-111">[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) collection</span></span>|<span data-ttu-id="4489e-112">Получите список объектов [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="4489e-112">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>|
|[<span data-ttu-id="4489e-113">Get cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="4489e-113">Get cloudPcConnection</span></span>](../api/managedtenants-cloudpcconnection-get.md)|[<span data-ttu-id="4489e-114">microsoft.graph.managedTenants.cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="4489e-114">microsoft.graph.managedTenants.cloudPcConnection</span></span>](../resources/managedtenants-cloudpcconnection.md)|<span data-ttu-id="4489e-115">Ознакомьтесь с свойствами и отношениями объекта [cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)</span><span class="sxs-lookup"><span data-stu-id="4489e-115">Read the properties and relationships of a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4489e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="4489e-116">Properties</span></span>
|<span data-ttu-id="4489e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="4489e-117">Property</span></span>|<span data-ttu-id="4489e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4489e-118">Type</span></span>|<span data-ttu-id="4489e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4489e-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4489e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4489e-120">displayName</span></span>|<span data-ttu-id="4489e-121">String</span><span class="sxs-lookup"><span data-stu-id="4489e-121">String</span></span>|<span data-ttu-id="4489e-122">Отображение имени облачного подключения к КОМПЬЮТЕРУ.</span><span class="sxs-lookup"><span data-stu-id="4489e-122">The display name of the cloud PC connection.</span></span> <span data-ttu-id="4489e-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4489e-123">Required.</span></span> <span data-ttu-id="4489e-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-124">Read-only.</span></span>|
|<span data-ttu-id="4489e-125">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="4489e-125">healthCheckStatus</span></span>|<span data-ttu-id="4489e-126">String</span><span class="sxs-lookup"><span data-stu-id="4489e-126">String</span></span>|<span data-ttu-id="4489e-127">Состояние здоровья облачного подключения к ПК.</span><span class="sxs-lookup"><span data-stu-id="4489e-127">The health status of the cloud PC connection.</span></span> <span data-ttu-id="4489e-128">Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4489e-128">Possible values are: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span></span>  <span data-ttu-id="4489e-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4489e-129">Required.</span></span> <span data-ttu-id="4489e-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-130">Read-only.</span></span>|
|<span data-ttu-id="4489e-131">id</span><span class="sxs-lookup"><span data-stu-id="4489e-131">id</span></span>|<span data-ttu-id="4489e-132">String</span><span class="sxs-lookup"><span data-stu-id="4489e-132">String</span></span>|<span data-ttu-id="4489e-133">Уникальный идентификатор для облачного подключения к ПК.</span><span class="sxs-lookup"><span data-stu-id="4489e-133">The unique identifier for the cloud PC connection.</span></span> <span data-ttu-id="4489e-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4489e-134">Required.</span></span> <span data-ttu-id="4489e-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-135">Read-only.</span></span>|
|<span data-ttu-id="4489e-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="4489e-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="4489e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4489e-137">DateTimeOffset</span></span>|<span data-ttu-id="4489e-138">Дата и время последнего обновления объекта на платформе управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="4489e-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="4489e-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4489e-139">Required.</span></span> <span data-ttu-id="4489e-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-140">Read-only.</span></span>|
|<span data-ttu-id="4489e-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="4489e-141">tenantDisplayName</span></span>|<span data-ttu-id="4489e-142">String</span><span class="sxs-lookup"><span data-stu-id="4489e-142">String</span></span>|<span data-ttu-id="4489e-143">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="4489e-143">The display name for the managed tenant.</span></span> <span data-ttu-id="4489e-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4489e-144">Required.</span></span> <span data-ttu-id="4489e-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-145">Read-only.</span></span>|
|<span data-ttu-id="4489e-146">tenantId</span><span class="sxs-lookup"><span data-stu-id="4489e-146">tenantId</span></span>|<span data-ttu-id="4489e-147">String</span><span class="sxs-lookup"><span data-stu-id="4489e-147">String</span></span>|<span data-ttu-id="4489e-148">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="4489e-148">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="4489e-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4489e-149">Required.</span></span> <span data-ttu-id="4489e-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4489e-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4489e-151">Связи</span><span class="sxs-lookup"><span data-stu-id="4489e-151">Relationships</span></span>
<span data-ttu-id="4489e-152">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4489e-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4489e-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4489e-153">JSON representation</span></span>
<span data-ttu-id="4489e-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4489e-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
